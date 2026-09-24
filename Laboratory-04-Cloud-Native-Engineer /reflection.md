# Mission Reflection — Cloud-Native Engineer

## 1. Boot Time Comparison
A Docker container starts in seconds because it shares the host's operating system kernel — there is no need to initialize a separate OS, drivers, or services. In contrast, installing and booting a Virtual Machine takes minutes because the VM must load its own full guest operating system from scratch, just like a physical computer. This speed means containers can scale instantly when traffic increases.

## 2. Purpose of Port Mapping
Port mapping (`-p 8080:80`) connects a port on your host machine to a port inside the container. Multiple containers can run on the same host without conflicting — each uses a unique external port even if they all use port 80 internally. Without this mapping, the containerized web server would be isolated and inaccessible from outside its own network.

## 3. Data When Using `docker rm`
When you delete a container with `docker rm`, any data stored inside that specific container filesystem is permanently erased unless you used a **volume** to persist it. Containers are designed to be stateless and disposable by default — they can be created and destroyed without losing critical data if volumes are configured properly.

## 4. Impact on DevOps
Containerization unifies development and operations teams — developers build and test containers that run identically in production. This eliminates "it works on my machine" problems and accelerates software delivery. Developers focus on code; operations teams focus on infrastructure — containers bridge the gap so both teams work toward the same deployable artifacts.

## 5. GitHub Portfolio Growth
My portfolio now demonstrates practical engineering skills — not just theory. I can research, execute commands, troubleshoot, and document real cloud tools. The organized structure shows I can follow professional workflows, and the consistent documentation style prepares me for real-world cloud engineering roles.
