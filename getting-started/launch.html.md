---
title: "Getting Started"
objective: Deploy any app to Fly.io in 15 minutes
layout: navigable_docs
order: 1
---

<figure class="w:full mt:6">
  <img src="/static/images/speedrun.webp" srcset="/static/images/speedrun@2x.webp 2x" alt="">
</figure>

You have an application you want to deploy on Fly.io as quickly as possible? You're in the right place. You'll have your app up and running in just three steps:

## [1. Install the `flyctl` Command Line Tool](launch/install)

Fly applications are deployed and managed with the `flyctl` command line tool, which you can install on any of these operating systems.

<div class="min-w-0 overflow-x-auto bg-white shadow-md rounded-xl lg:-mx-8 mb-7 ring-1 ring-gray-700 ring-opacity-10">
    <table class="table-stripe table-stretch table-pad text-sm whitespace-nowrap m-0">
        <thead class="text-navy text-left">
            <tr>
                <th>Operating System</th>
                <th>Installation Command</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>macOS</td>
                <td><code>brew install flyctl</code></td>
            </tr>
            <tr>
                <td>Linux</td>
                <td><code>curl -L https://fly.io/install.sh | sh</code></td>
            </tr>
            <tr>
                <td>Windows</td>
                <td><code>pwsh -Command "iwr https://fly.io/install.ps1 -useb | iex"</code></td>
            </tr>
        </tbody>
    </table>
</div>

## [2. Create a Fly.io Account](launch/log-in-to-fly)

You will create or login to your Fly.io account from the `flyctl` command line tool:

1. Create an account with `fly auth signup` or login with `fly auth login`.
2. Run `fly launch` from inside your project source directory - create, configure, and deploy a new application.

## [3. Launch the App](launch/launch)

`fly launch` can configure and deploy the following kinds of apps automatically:

* [Crystal](/docs/getting-started/crystal/)
* [Deno](/docs/getting-started/deno/)
* [Django](/docs/django/getting-started)
* [Elixir](/docs/elixir/getting-started)
* [Go](/docs/getting-started/golang/)
* [Node](/docs/getting-started/node/)
* [Laravel](/docs/getting-started/laravel/)
* [Python](/docs/getting-started/python/)
* [Rails](/docs/getting-started/rails/)
* [RedwoodJS](/docs/getting-started/redwood/)
* [Remix](/docs/getting-started/remix/)
* [NuxtJS](/docs/getting-started/nuxtjs/)
* [NextJS](/docs/getting-started/nextjs/)
* [Ruby](/docs/getting-started/ruby/)
* [Static Website](/docs/getting-started/static/)

You're not limited to these kinds of projects, though! `fly launch` also knows what to do [with a Dockerfile](/docs/languages-and-frameworks/dockerfile/), so you can use the tech _you_ love.

Refer to [Launch a new app](/docs/apps/launch/) to learn more about what `fly launch` does.

## [Working with Fly Apps](launch/working-with-fly-apps)

Once you deploy your app you'll want to see its status and open it so you can mange it.

1. Run `fly status` - show the status of the application instances.
2. Run `fly apps open` - open your browser and direct it to your app.

If things don't go as smoothly as you'd like, visit our [community forum](https://community.fly.io) and get help.

Would you like to know more?

* **Apps can store only ephemeral data in their root file systems.** Learn about [persistent storage options](/docs/database-storage-guides/).
* **You have control over how your app deploys and what resources it uses.** Learn about [Fly Apps](/docs/apps/).
* **Beyond just launching your app; go deeper with our most comprehensive framework guides.** Learn about [Elixir on Fly.io](/docs/elixir), [Rails on Fly.io](/docs/rails/), [Laravel on Fly.io](/docs/laravel/), and [Django on Fly.io](/docs/django).

It's also easy to [bring your Heroku app to Fly.io](/launch/turboku). Read more about it in the [Turboku launch post](https://fly.io/blog/new-turboku/).

Check out our other [Web Launchers](/launch), too.