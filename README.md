# schb-microservice

Rug generator to create basic Space Corps Handbook Micorservices project structure

See the [Rug documentation][rug] for more information on Rug Archives.

[rug]: http://docs.atomist.com/

## Rugs

### AddReadme

The AddReadme Editor adds a GitHub-like `README.md` to a project.

#### Prerequisites

Before running this Editor, you must have the following prerequisites
satisfied.

*   A source code repository

#### Parameters

To run this editor, you must supply the following parameters.

Name | Required | Default | Description
-----|----------|---------|------------
`project_name` | Yes | | A valid GitHub repository name.  It must be 21 characters or less to avoid truncating name when the its Slack channel is created.
`description` | No | My new project | A brief description of the project with at least one character and fewer than 90.

[semver]: http://semver.org

#### Running

Run it as follows:

```
$ cd to/the/repo
$ rug edit org.spacecorpshandbook:schb-microservice:AddReadme \
    project_name=fun-project \
    description="A project that needs a README"
```

This will create a simple `README.md` file in the top-level directory
of the source code repository.  If you are happy with the change,
commit the changes.

## Support

If you find a problem, please create an [issue][].

[issue]: https://github.com/org.spacecorpshandbook/schb-microservice/issues

## Development

You can build, test, and install the project locally with
the [Rug CLI][cli].

[cli]: https://github.com/atomist/rug-cli

```
$ rug test
$ rug install
```

---
Created on  by [Atomist][atomist].
Need Help? [Join our Slack community][slack].

[atomist]: https://www.atomist.com/
[slack]: https://join.atomist.com/
