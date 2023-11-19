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
| [static-rust](https://actix.rs/) | Rust | Actix Web | 1.86ms | 110kps |
| [Tailcall](https://tailcall.run/) | Rust | Hyper | 3.09ms | 65kps |
| [graphql-crystal](https://github.com/graphql-crystal/graphql) | Crystal | Kemal | 3.28ms | 62kps |
| [gqlgen](https://github.com/99designs/gqlgen) | Go | net/http | 4.27ms | 47kps |
| [async-graphql](https://github.com/async-graphql/async-graphql) | Rust | Actix Web | 4.43ms | 45kps |
| [Juniper](https://github.com/graphql-rust/juniper) | Rust | Actix Web | 5.39ms | 37kps |
| [Hot Chocolate](https://github.com/ChilliCream/hotchocolate) | C# | ASP.NET | 8.64ms | 23kps |
| [Mercurius](https://github.com/mercurius-js/mercurius) | Node.js | Fastify | 9.99ms | 20kps |
| [graphql-go](https://github.com/graphql-go/graphql) | Go | net/http | 10.98ms | 18kps |
| [graphql-yoga](https://github.com/dotansimha/graphql-yoga) | Node.js | http | 14.79ms | 14kps |
| [agoo](https://github.com/ohler55/agoo) | Ruby/C | agoo | 18.79ms | 11kps |
| [nim-graphql](https://github.com/status-im/nim-graphql) | Nim | Chronos | 19.73ms | 10kps |
| [graphql-jit](https://github.com/zalando-incubator/graphql-jit) | Node.js | http | 20.05ms | 10.0kps |
| [Absinthe](https://github.com/absinthe-graphql/absinthe) | Elixir | Phoenix | 23.78ms | 8.4kps |
| [Hono](https://github.com/honojs/graphql-server) | Bun | HonoJS | 28.03ms | 7.1kps |
| [apollo](https://github.com/apollographql/apollo-server) | Node.js | Express | 34.33ms | 5.8kps |
| [graphql-ruby](https://github.com/rmosolgo/graphql-ruby) | Ruby | Puma | 44.43ms | 5.8kps |
| [graphql-js](https://github.com/graphql/graphql-js) | Node.js | http | 48.70ms | 4.1kps |
| [Sangria](https://github.com/sangria-graphql/sangria) | Scala | Akka HTTP | 90.58ms | 2.2kps |
| [Strawberry](https://github.com/strawberry-graphql/strawberry) | Python | gunicorn | 107.49ms | 1.8kps |
| [Graphene](https://github.com/graphql-python/graphene) | Python | gunicorn | 107.67ms | 1.8kps |
