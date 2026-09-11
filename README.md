# Food Delivery System — Bruno Collection

Bruno API collection for a food delivery system. Designed for team collaboration via Git.

Built for the educational project [go-mentor-junior](https://github.com/meetmorrowsolonmars/go-mentor-junior).

## Structure

```
Order/          — Order Service (localhost:8080)
  Customer/     — customer actions (cart, orders)
  Restaurant/   — restaurant actions on orders (accept, reject, prepare)
Restaurant/     — Restaurant Service (separate service)
environments/   — environment variables (Local.yml)
```

## Prerequisites

- [Bruno](https://github.com/usebruno/bruno) — open-source API client (download the desktop app from the releases page)
- Git

## Getting Started

```bash
git clone git@github.com:zulerne/bruno-food-delivery-system.git
cd bruno-food-delivery-system
```

In Bruno:

1. **Open Collection** → select the `bruno-food-delivery-system` folder (where `opencollection.yml` lives)
2. Select the **Local** environment
3. Start the relevant Go service locally and send requests

> The `order_url` variable in the Local environment points to `localhost:8080` — the service must be running on your machine.

## Collaboration

Before making changes (clean working tree):

```bash
git pull --ff-only
```

After editing requests in Bruno:

```bash
git add .
git commit -m "feat: add ..."
git push
```

Your teammate runs `git pull --ff-only` and gets the updated collection without re-importing it.
