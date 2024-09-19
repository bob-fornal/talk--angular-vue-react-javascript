# Comparing Angular, Vue, React, and JavaScript

This repository will consist of several folders. Each will be a different part of the comparison.

## Base Code

The idea of this will take one **CONCEPT** and build an application around it in each area (groups).

Since there are several ways to implement a React or JavaScript solution, there will most likely be more than 4 options (implementations). Versioning should be included in the folder names to ensure that this repository can grow over time.

There should be a base node-server that can be used to test various implementations consistently.

The core project should:

* Implement a "component;" something complicated enough to add a level complexity.
* Implement paging or routing.
* Investigate TypeScript versus JavaScript in the implementations.

### Component

The component will be:

* A routing/ab-test component that will provide an option to link to the root.
* It will also show the route and/or percent and routes.

```
http://www.root-site.com/route1/
  |- /routing-to-this-page/

http://www.root-site.com/ab-test-route/
  |- 80% /routing-80-percent-here/
  |- 20% /routing-20-percent-here/
```

### Paging

Paging should take into account various implementation options and determine when or where `hashrouting` might be necessary.

## Analysis

The core analysis data will be built into each implementation and incorporated into a higher level summary; again, taking versioning into account.

The analysis needs to look into / explore implementations:

* Individual Needs
* Single Team Organization (one frontend developer)
* Mid-Sized Organizations (2-3 frontend developers)
* Enterprise-Level Organizations (multiple teams of developers)

The analysis should also account for:

* Internal Applications
* External Applications
