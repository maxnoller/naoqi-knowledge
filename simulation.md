## Simulation

### Why you cant connect to your robot using nao.local when you are running naoqi-bin as a simulation
Pretty easy took me way to long to figure out, you gotta install avahi daemon

### Why can't I connect to ALAutonomousLife when I am running the simulation in a docker container
Idk it fucks the endpoints of the legacy services like ALAutonomousLife up, I havent fully tested this yet but I think you can fix this by installing the avahi daemon and connecting over the .local domain
