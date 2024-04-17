---
layout: default
---
Hey! 👋

If you ended up here is probably because you're looking for your own small space in the Software Engineering universe.

Whether you are interested in creating a space with your thoughts, or you might have an interesting idea you decided to 
pursue, a `.software-engineer.space` domain might be exactly what you need.

## Getting your `.software-engineer.space`

Let's say you want to host your simple static website to sustain your new idea
under `your-domain.software-engineer.space`, then create a PR (through `your-github-username`) in
the [`software-engineer.space-terraform` repository](https://github.com/software-engineer-space/software-engineer.space-terraform)
which adds to
the [`spaces` variable](https://github.com/software-engineer-space/software-engineer.space-terraform/blob/main/spaces.tf#L2)
an entry with the following shape

```terraform
{
github_handle = "your-github-username"
dns_prefix = "your-domain"
}
```

Whenever possible the PR will be merged and the changes applied. As a result `your-github-user` GitHub user will be
assigned with the permissions to write on the newly created `your-domain.sofware-engineer.space` repository in order to
modify the content of the website.

## Supported use-cases

The only available service for the moment is the GitHub hosted website described above.

If you have other scenarios or special requests feel free to open an issue, I'd be happy to help and understand your
needs.

## Why are you doing this?
I was playing around with managing Cloudflare DNS via Terraform and I wanted a place where to store my configurations
and the obvious answer was GitHub. But why create repositories manually if I could have used Terraform for it as well?

That's how the idea was born.

Speaking of the hype cycle I haven't probably reached yet the "peak of inflated expectations" so,
as far as I'm learning, I'm happy.

The bubble will pop inevitably, but that'd still be learning, right?
