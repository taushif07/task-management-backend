# task-management-backend

{
  "version": 2,
  "builds": [
    {
      "src": "index.js",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    { "src": "/todos", "dest": "index.js" },
    { "src": "/(.*)", "dest": "index.js" }
  ],
  "env": {
    "MONGO_URL": "mongodb+srv://taushif07:FYzrGf79gm98EKc7@cluster0.bonshpl.mongodb.net/Tasks?retryWrites=true&w=majority",
    "PUBLIC_DIR": "public",
    "PORT": 8080
  }
}
