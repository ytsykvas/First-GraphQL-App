# README

# Simple project with realized Rails graphQL API 

## Start
* clone repository
```
git clone https://github.com/username/project.git
```

* install dependencies
```
bundle install
```
* creating and seeding DB
```
rails db:create db:migrate db:seed
```
You will have 4 ready to use items to work with.
* run project
```
rails server
```
Your local project will be ready to use GraphQL requests at 
```
http://localhost:3000/graphiql
```
## How to make a request?
* Get seeded items
At http://localhost:3000/graphiql enter next data to get all items:
```
{
  items {
    id
    title
    description
    artist {
      firstName
      email
      createdAt
    }
  }
}
```
