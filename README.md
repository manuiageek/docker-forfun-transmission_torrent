# Service Transmission
- Image: linuxserver/transmission
- Container Name: transmission
- Restart Policy: unless-stopped

# Usage
## To start the Transmission container, use the following command:
```
docker-compose up -d
```
**_This command will start the Transmission service in detached mode._**

# Access
After starting the container, you can access the Transmission web interface  
by navigating to `http://<your-server-ip>:9091` in your web browser.

# Notes
- Ensure the specified directories for volumes exist on your host machine.
- Adjust the USER and PASS environment variables to secure your Transmission web interface.
- Modify the PUID and PGID variables if necessary to match your system's user and group IDs.
- This configuration ensures a controlled resource usage for the Transmission service, providing a balance between performance and efficiency.
- The value 0.5 indicates a fraction of the total available CPU on the host. If your host has 4 CPUs, the container can use the equivalent of 2 CPUs (4 * 0.5).
