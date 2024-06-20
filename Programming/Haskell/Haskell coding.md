Suppose you are using cabal run as a way to compile and run your code. If you have a Main.hs that depends on other modules you have defined these are some rules that you should follow for peace of mind

### 1. Import syntax

In the Main.hs the import syntax should look like
```
import Particle (Particle(..), Swarm(..), updateVelocity, updatePosition, updateCost, updateSwarm)
```

In the Particle.hs the export syntax should look like
```
module Particle (Particle(..), Swarm(..), updateVelocity, updatePosition, updateCost, updateSwarm)
```

Note that if you have to import a module in Particle.hs it should stated below the export statement
```
module Particle (Particle(..), Swarm(..), updateVelocity, updatePosition, updateCost, updateSwarm)
import Data.List (<functions etc>)
```

### 2. Using imported data structures
If you have a imported data structure example Particle in
```
import Particle (Particle(..), Swarm(..), updateVelocity, updatePosition, updateCost, updateSwarm)
```

To use it you must explicitly give values to the internal structures
```
p :: Particle
p = Particle {position = ..., velocity = ..., .....}
```
