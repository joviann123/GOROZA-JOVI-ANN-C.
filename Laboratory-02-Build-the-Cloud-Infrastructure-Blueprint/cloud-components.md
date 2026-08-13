# Cloud Infrastructure Components Analysis

### 1. Compute Resources
*   **Purpose:** Responsible for executing instructions, running applications, and processing computational workloads.
*   **Importance in Cloud:** Compute forms the engine of the cloud; without it, applications cannot execute logic or serve user requests dynamically.
*   **Linux Environment Relation:** Witnessed in the KillerCoda sandbox via allocated virtual CPU cores (`lscpu`) and volatile memory components (`free -h`).

### 2. Storage Resources
*   **Purpose:** Provides persistent and non-persistent locations to save configuration settings, databases, and application system binaries.
*   **Importance in Cloud:** Cloud infrastructure relies heavily on scaling decoupled storage arrays to ensure data persists even if virtual machine instances crash or cycle out.
*   **Linux Environment Relation:** Observed in our workspace through block file system mounts mapped on the root path `/` verified via the `df -h` command.

### 3. Networking Resources
*   **Purpose:** Establishes communication pathways, routing data safely between cloud servers, external backends, and the public internet.
*   **Importance in Cloud:** It defines the secure environment (subnets, firewalls, gateways) that prevents raw exposure of infrastructure assets directly to external bad actors.
*   **Linux Environment Relation:** Handled via the virtual network interfaces bound to the private/public IP addresses extracted through `hostname -I`.

### 4. Operating System
*   **Purpose:** The baseline software layer abstracting complex physical hardware architectures into standard runtime environments for apps.
*   **Importance in Cloud:** Provides a consistent, automated environment for deployment pipelines, scripting languages, and system runtimes.
*   **Linux Environment Relation:** Found as the active distribution powering our entire live session workspace (`/etc/os-release`).
