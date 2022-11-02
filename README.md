## Reusable Workflows

There are 3 workflows here designed to be used by other repos. You can use them this way:

For a .NET Docker build
```yaml
  docker:
    uses: BoxBoat-Codespaces/my-workflows/.github/workflows/dotnet-docker.yml@main
    with:
      tag: my-tag
    secrets: inherit
```

To deploy a Container App
```yaml
  terraform:
    uses: BoxBoat-Codespaces/my-workflows/.github/workflows/terraform.yml@main
    with:
      tag: my-tag
    secrets: inherit
```

To run an API Smoke Test
```yaml
  test:
    uses: BoxBoat-Codespaces/my-workflows/.github/workflows/newman.yml@main
    with:
      url: baseUrl
```
