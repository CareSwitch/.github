## 💡 What we do

Careswitch is building the world’s largest network of home care providers, caregivers, families, clients, and partners to create a more stable, coordinated home care experience for all.

We do this by building shared tools and common practices to create more consistency and transparency in the home care experience. Together, we leverage our collective scale to unlock more economic opportunity and improve quality of life for everyone in the home care community.

## 🔧 Our stack

- Relay API using Postgres, [Hasura](https://hasura.io)
- ReScript React web app using [Next.js](https://nextjs.org), [Relay](https://rescript-relay-documentation.vercel.app/docs/making-queries), [Tailwind](https://tailwindcss.com)
- ReScript React Native app using Relay, Tailwind

[ReScript](https://rescript-lang.org) is a statically typed language based on OCaml that compiles to efficient JavaScript and integrates tightly with React—here's a sample `Button` component:

```res
module Button = {
  type kind = Primary | Secondary

  @react.component
  let make = (~kind, ~children) => {
    let className = switch kind {
      | Primary => "p-4 bg-blue text-lg"
      | Secondary => "p-2 bg-gray-2 text-base"
    }
    <button className> children </button>
  }
}

<Button kind=Button.Secondary>
  {React.string("Press me")}
</Button>
```

Interested? [We're hiring](https://www.careswitch.com/careers?gh_jid=4029827004).
