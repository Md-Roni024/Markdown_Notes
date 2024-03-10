- What is express.js?
    - Express.js is a minimal and flexible framework for node.js to create and maintain server more easily.
- Setup Vscode for express.js
    - first init npm by this command
      ```
      npm init -y  //Default Setup
      npm init    //custom setup for name,version,entrypoint
      ```

- Why nodemon is used?
    - Nodemon is a tool which reastart server automatically if any changes is detect in directory.

- Install express.js and nodeamon
    ```
    node install express nodemon
    ```
- package.json, package.lock.json and node_modules

- http methods:
    - get,post,put,delete,patch
    - get method:
      ```js
      app.get("/",(req,res)=>{
       res.send("I am at Home Route")
      });

      app.post("/",(req,res)=>{
            res.send("I am at Post Route")
      });

      app.put("/",(req,res)=>{
            res.send("I am at Put Route")
      });

      app.delete("/",(req,res)=>{
            res.send("I am at delete Route")
      });

      ```

- Can send {String,HTML,JSON,Coockies} as response to api
- Send Parameter to server by
    - Query Parameter
    - Route Parameter
    - Request Header


- npm JSON Parser
- Area Calculator
- Regular expression
- Set .env file


- MiddleWare and Types
- Static Midddlware