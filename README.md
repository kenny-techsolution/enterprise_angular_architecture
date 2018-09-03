# enterprise_angular_architecture

architecture principle

architecture aspect
## folder structure
* locate code quickly
* near-term view
* long-term vision
* simplier dependency graph
* scalable

### structure 
#### Feature module
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
    -- resolvers/
    -- guards/

#### core module
* used only once
* used globally
* used by root app
* singleton service

-- core
    -- auth/
    -- http/
    
