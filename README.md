<!-- README.md is generated from README.ecr, do not edit -->

# GraphQL server benchmarks

Graphql server benchmarks in many languages. Pull requests welcome, please read [CONTRIBUTING.md](CONTRIBUTING.md)

All servers implement a simple schema:

```graphql
type Query {
  hello: String!
}
```

The returned string is always `world`.

The API is served over HTTP using a common web server and load tested using [bombardier](https://github.com/codesenberg/bombardier).

### Results

| Name                          | Language      | Server          | Latency avg      | Requests      |
| ----------------------------  | ------------- | --------------- | ---------------- | ------------- |
| [static-rust](https://actix.rs/) | Rust | Actix Web | 1.83ms | 110kps |
| [Tailcall](https://tailcall.run/) | Rust | Hyper | 3.03ms | 66kps |
| [graphql-crystal](https://github.com/graphql-crystal/graphql) | Crystal | Kemal | 3.34ms | 60kps |
| [gqlgen](https://github.com/99designs/gqlgen) | Go | net/http | 3.96ms | 51kps |
| [async-graphql](https://github.com/async-graphql/async-graphql) | Rust | Actix Web | 4.60ms | 43kps |
| [Juniper](https://github.com/graphql-rust/juniper) | Rust | Actix Web | 4.92ms | 41kps |
| [Hot Chocolate](https://github.com/ChilliCream/hotchocolate) | C# | ASP.NET | 8.58ms | 23kps |
| [Mercurius](https://github.com/mercurius-js/mercurius) | Node.js | Fastify | 9.90ms | 20kps |
| [graphql-go](https://github.com/graphql-go/graphql) | Go | net/http | 10.99ms | 18kps |
| [graphql-yoga](https://github.com/dotansimha/graphql-yoga) | Node.js | http | 14.89ms | 13kps |
| [graphql-jit](https://github.com/zalando-incubator/graphql-jit) | Node.js | http | 20.05ms | 10.0kps |
| [nim-graphql](https://github.com/status-im/nim-graphql) | Nim | Chronos | 20.65ms | 9.7kps |
| [Absinthe](https://github.com/absinthe-graphql/absinthe) | Elixir | Phoenix | 23.96ms | 8.3kps |
| [agoo](https://github.com/ohler55/agoo) | Ruby/C | agoo | 26.61ms | 7.3kps |
| [Hono](https://github.com/honojs/graphql-server) | Bun | HonoJS | 28.55ms | 7.0kps |
| [apollo](https://github.com/apollographql/apollo-server) | Node.js | Express | 34.78ms | 5.8kps |
| [graphql-ruby](https://github.com/rmosolgo/graphql-ruby) | Ruby | Puma | 44.67ms | 5.7kps |
| [graphql-js](https://github.com/graphql/graphql-js) | Node.js | http | 45.94ms | 4.4kps |
| [Sangria](https://github.com/sangria-graphql/sangria) | Scala | Akka HTTP | 90.91ms | 2.2kps |
| [Strawberry](https://github.com/strawberry-graphql/strawberry) | Python | gunicorn | 108.45ms | 1.8kps |
| [Graphene](https://github.com/graphql-python/graphene) | Python | gunicorn | 108.37ms | 1.8kps |
