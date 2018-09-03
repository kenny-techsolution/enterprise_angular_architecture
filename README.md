# enterprise_angular_architecture

architecture principle

scalable. easy to extend feature. 
simpler dependency graph.

architecture aspect
## folder structure
* locate code quickly
* near-term view
* long-term vision

### structure 
#### feature module
* don't depend on another feature module
* only depend on shared module

-- features/
    -- product/
        -- components/
        -- pages/
        -- product-routing.module.ts
        -- project.module.ts

#### shared module
* used in more than one module
* imported by feature module

-- shared
    -- components/
    -- directives/
    -- pipes/

#### core module
* used only once
* used globally
* used by app

-- core
    -- auth/
    -- http/
