[ 𝐑𝐄𝐒𝐓 (𝐑𝐞𝐩𝐫𝐞𝐬𝐞𝐧𝐭𝐚𝐭𝐢𝐨𝐧𝐚𝐥 𝐒𝐭𝐚𝐭𝐞 𝐓𝐫𝐚𝐧𝐬𝐟𝐞𝐫) ]

⚠ Architectural Style, Not a Protocol.

REST is not a strict protocol, but rather a set of architectural principles outlined by Roy Fielding in his doctoral dissertation.

REST is a set of guidelines for structuring web APIs.

REST aims to be a simple and lightweight approach to API design.

◾ REST APIs are built around resources, with clear and hierarchical URLs for accessing them.

For example, /users/123 in a REST API would represent a user with ID 123.

HTTP at its Core.

◾ REST heavily leverages existing HTTP methods (GET, POST, PUT, DELETE) to perform actions on resources.

GET - Retrieves a representation of a resource
POST - Creates a new resource
PUT - Updates an existing resource
DELETE - Removes a resource

◾ One core principle of REST is statelessness. Each REST request is independent, and the server doesn't maintain client context between requests.

This aids scalability.

◾ REST responses should indicate whether they can be cached, improving performance for subsequent requests for the same data.

📌 If your API primarily deals with CRUD (Create, Read, Update, Delete) operations on straightforward individual resources, REST's resource-centric approach is a natural fit.


[ 𝐆𝐫𝐚𝐩𝐡𝐐𝐋 ]

GraphQL is more than just a query language.

It's a runtime environment that allows clients to request specific data from a server using a flexible query language.

◾ GraphQL offers a specification for defining API schemas and a powerful query language for client-server communication.

◾ GraphQL views data as a graph of interconnected nodes (entities) and edges (relationships).

This allows fetching complex, nested data structures.

◾ Clients send GraphQL queries describing precisely the data they require.

◾ GraphQL enforces a strong type system through a schema that defines the capabilities of an API.

GraphQL's schema can be extended over time without breaking existing clients, provided you don't remove previously used fields.

📌 Use GraphQL when your application has a highly connected data model with various relationships. It can fetch nested data in a single request, which REST may require multiple round trips to achieve.

[ 𝐂𝐫𝐢𝐭𝐢𝐜𝐚𝐥 𝐈𝐧𝐬𝐢𝐠𝐡𝐭𝐬 ]

1. REST and GraphQL can coexist within an application and are not necessarily mutually exclusive.

2. REST often leads to over-fetching (more data than needed) or under-fetching (multiple requests). GraphQL minimizes these issues.

3. GraphQL's flexibility can introduce a potential for slower query resolution on very complex backend systems if not carefully optimized.

4. REST offers a simpler structure. GraphQL is more powerful but comes with a steeper learning curve.

![image](https://github.com/r-shreesha/Interview-Prep/blob/main/Design_Diagrams/Rest%20vs%20GraphQL.gif)
