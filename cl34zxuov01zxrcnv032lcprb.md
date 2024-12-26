---
title: "What is Declaration merging in Typescript?"
datePublished: Fri May 13 2022 22:13:43 GMT+0000 (Coordinated Universal Time)
cuid: cl34zxuov01zxrcnv032lcprb
slug: what-is-declaration-merging-in-typescript-1
canonical: https://medium.com/@abdulshekurabdullahclement/what-is-declaration-merging-in-typescript-d0eff9430b5f
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670688836682/m6diZUT6G.jpeg
tags: javascript, typescript

---

## **What is Declaration merging in typescript?**

*   **Explanation:**
    
    In typescript, a value, a type and a namespace can be stacked on each other as a single entity and exported out with a single identifier.
    

> [*💡Namespace-creating declarations create a namespace, which contains names that are accessed using a dotted notation. Type-creating declarations do just that: they create a type that is visible with the declared shape and bound to the given name. Lastly, value-creating declarations create values that are visible in the output JavaScrip*](https://devdocs.io/typescript/declaration-merging#basic-concepts)

| Declaration Type | Namespace | Type | Value |
| --- | --- | --- | --- |
| Namespace | X |  | X |
| type alias |  | X |  |
| interface |  | X |  |
| class |  | X | X |
| enum |  | X | X |
| function |  |  | X |
| variable |  |  | X |

*   **Merging Interfaces**
    
    Interfaces are the most common declaration merging type in typescript, members of the declared interface types are simply merged into a single interface and assigned a single identifier.
    
    ```typescript
    interface User{
    	id: number;
    	name: string;
    	job: string;
    	salary: string;
    }
    
    interface User {
    	gender: string;
    	isMarried: boolean;
    
    }
    
    const user: User = {
    id: 3, 
    name: "Abdul Shakur", 
    job: "software developer",					        
    salary: $4000, 
    gender: "male", 
    isMarried: true 
    }
    ```
    
    **Note**: The last interface always has the highest precedence when merging.
    
    > [*For function members, each function member of the same name is treated as describing an overload of the same function. Of note, too, is that in the case of interface*](https://devdocs.io/typescript/declaration-merging#basic-concepts) `A` merging with a later interface `A`, the second interface will have higher precedence than the first.
    
    ```typescript
    interface Document {
      createElement(tagName: any): Element;
    }
    interface Document {
      createElement(tagName: "div"): HTMLDivElement;
      createElement(tagName: "span"): HTMLSpanElement;
    }
    interface Document {
      createElement(tagName: string): HTMLElement;
      createElement(tagName: "canvas"): HTMLCanvasElement;
    }
    ```
    
    The resulting merged declaration of `Document` will be as follows
    
    ```typescript
    interface Document {
      createElement(tagName: "canvas"): HTMLCanvasElement;
      createElement(tagName: "div"): HTMLDivElement;
      createElement(tagName: "span"): HTMLSpanElement;
      createElement(tagName: string): HTMLElement;
      createElement(tagName: any): Element;
    }
    ```
    
*   **Merging Namespaces**
    
    Namespace with the same name will merge their members and export as single entity. We need to understand that namespaces create a namespace and a value.
    
    To merge the `namespaces`, the type definitions exported interfaces declared in each namespace are themselves merged, to form a single namespace with merged type definitions in it.
    
    To merge the `namespace` `value,` once a namespace with the same name already exists, typescript will maintain the existing namespace and only extend it by adding the members of the subsequent namespaces, with the same name, to the first namespace.
    
    *Code Example:*
    
    ```typescript
    namespace UsersDB{
      export class AdminUser {}
    }
    
    namespace UsersDB {
    
    // un-exported type declaration
    interface Staff {
      staffID: number;
      name: string;
      role: string[];
      salary?: string;
      department: string;
    
    }
    
    // exported type declaratio
     export interface User {
      id: number;
      name: string;
      job: string;
      salary: string;
     }
    
    // exported type declaration
     export class ClientUser{}
    
    }
    ```
    
    > [This model of namespace merging is a helpful starting place, but we also need to understand what happens with non-exported members. Non-exported members are only visible in the original (un-merged) namespace. This means that after merging, merged members that came from other declarations cannot see non-exported members.](https://devdocs.io/typescript/declaration-merging#basic-concepts)
    
    When the code snippets above are merged, the code below will be the result;
    
    ```typescript
    namespace UsersDB {
      export interface User {
        id: number;
        name: string;
        job: string;
        salary: string;
      }
      export class AdminUser {}
      export class ClientUser {}
    
    }
    ```
    
*   **Merging Namespaces with classes**
    
    The TS Compiler will merge members of a class and a namespace if they both have the same name. The members have to be exported in other to be recognized in the merged type declaration.
    
    ```typescript
    class ClientsDB {
      client!: ClientsDB.ClientName;
    }
    
    namespace ClientsDB {
      export class ClientName{
    
      }
    }
    ```
    
*   [**Merging Namespaces with function**](https://www.typescript-trainng.com/course/intermediate-v1/02-declaration-merging/)
    
    We could define a function and a namespace that “stack” like this, so that `$`  could simultaneously be invoked directly, and serve as a namespace for things like  `$.ajax`, `$.getJSON` and so on…
    
    ```typescript
    function $(selector: string): NodeListOf<Element> {
      return document.querySelectorAll(selector)
    }
    namespace $ {
      export function ajax(arg: {
        url: string
        data: any
        success: (response: any) => void
      }): Promise<any> {
        return Promise.resolve()
      }
    }
    ```