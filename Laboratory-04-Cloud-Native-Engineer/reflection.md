# Mission Reflection: Cloud-Native Engineering

The deployment speed and resource efficiency of Docker containers present a radical shift compared to traditional Virtual Machine provisioning. Setting up a Virtual Machine requires hypervisor allocation, operating system installation, dependency updates, and configuration—a process taking anywhere from several minutes to hours. In contrast, running a Docker container like Nginx takes mere seconds because it bypasses guest operating system initialization by directly sharing the host Linux kernel.

Port mapping (`-p 8080:80`) is crucial when running containerized applications because containers exist in isolated network namespaces. By default, port 80 inside the container is hidden from the host system. Port mapping creates a network bridge, directing traffic hitting host port 8080 into port 80 of the container, thereby allowing external users to access the web service.

When executing the `docker rm` command, the isolated writable container layer is permanently deleted. Any ephemeral data created inside the container during runtime is lost unless persistent storage volumes were attached. This highlights the importance of maintaining stateless container architectures where data persistence is handled by external database systems or persistent volume mounts.

Containerization fundamentally transforms DevOps collaboration by bridging the gap between developers and IT operations teams. Through container images, developers package code along with all system dependencies, ensuring that the application executes identically across development, staging, and production environments—effectively resolving the classic "it works on my machine" dilemma.

My GitHub cloud portfolio is continuously evolving into a comprehensive technical repository. By adding hands-on containerization and Docker management alongside multi-cloud evaluation documentation, it demonstrates a complete progression from cloud infrastructure exploration to modern cloud-native engineering practices.
