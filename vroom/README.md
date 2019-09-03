# Details
Docker Compose file for the "VROOM with OSRM backend" stack. You can solve *Vehicle Routing Problems* with just this file. 
This compose file consist of three Docker images:
- [OSRM](https://github.com/Project-OSRM/osrm-backend) used as *routing engine*.
- [VROOM Backend](https://github.com/iedmrc/vroom-docker) serves as a *Vehicle Routing Solver*. 
- [VROOM Frontend](https://github.com/iedmrc/vroom-frontend-docker) visualizes the routes calculated by the `VROOM Backend`.

Check the post [here](https://dev.to/iedmrc/vehicle-routing-problems-and-how-to-solve-them-8h3) for more details.