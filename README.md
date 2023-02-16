# nx pitch notes

## What is nx
- enterprise monorepo orchestration tooling and SAAS
- created by ex-Google engineers (Angular Maintainer) based on Google's Bazel

## Problems to solve

### Project tooling/dependency management
- nx manages all main project tooling/configuration and dependencies
- this frees developers from having to spend time researching the correct combination of dependencies that all work together

### Task running
- nx has built in task runner with advanced coordination abilities and caching
- tasks include linting, testing, formating, building, integration testing or any custom task we need
- replaces ad hoc script runner tooling with integrated task runners that understand the projects structure

### Highly coupled, monolithic applications
- facilitates the ability to break project apart into modularized packages that can be combined in arbitrary manners
- nx helps generate and orchestrate modularized node packages
- facilitates breaking app apart by feature, by page, by domain/subdomain
- facilitates micro front ends (see Micro Front Ends in resources for more info)
- modularizing and recombining packages to form the application allows for adept architectural changes. (i.e. moving from react router to nextjs)
- facilitates scoped development using storybook, features can be developed in isolation and then integrated into main app

### Long build/test cycles
- nx caches build results which can be shared amongst developers and ci/cd platforms
- dependency graph analysis, test/build only what changed
- incremental builds, build sub packages into final result, avoid re-building unchanged code

### Understanding structure of large code base
- by breaking project into many packages, we can trace the interconnections using dependency graph analysis
- visualize code structure using graphs
- facilitates operating on the affected path

### Lack of resources to look to when problems occur with tooling/project
- nrwl the creators of NX are a consulting company, you can pay them to help with whatever problems you're facing


## Alternatives to NX
- There are several monorepo coordination tools, but NX has the most features, support and is the only one with distributed task execution and SAAS support

## Risks
- Although well funded nrwl could fail, however nx is an open source project with nearly 20k stars on github and 3 million npm downloads a week, very likely support would be picked up by community or another company. Additionally, the nx tooling is mostly a thin layer on top of standardized JS tooling, bailing out to another monorepo tool or running a custom solution is probably reasonable.

## resources
- [nx techcrunch](https://techcrunch.com/2022/11/17/with-8-6m-in-seed-funding-nx-wants-to-take-monorepos-mainstream)
- [illustrated dte](https://nx.dev/more-concepts/illustrated-dte)
- [Micro Front Ends](https://techblog.geekyants.com/building-a-micro-frontend-using-react-and-angular)
- [Why Monorepos?](./why-monorepos.md)

## demos
- [large monorepo](https://github.com/vsavkin/large-monorepo)
- [dte](https://github.com/vsavkin/lerna-dte)

## DTE Image
![image](https://user-images.githubusercontent.com/16461670/219460948-da59f9f0-cdf9-480b-ab81-2580fdda9439.png)
