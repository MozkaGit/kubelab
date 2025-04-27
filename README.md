# 🏠 KubeLab

A personal Kubernetes lab for learning and experimentation.

## Introduction

This repository contains all the configuration and documentation of my personal Kubernetes laboratory (KubeLab).

The purpose of this KubeLab is to learn and have fun. As a DevOps/Cloud engineer, I work with Kubernetes daily, and this lab is where I can try out and learn new things. By self-hosting applications, I'm responsible for the entire process of deploying and maintaining applications from A to Z. This forces me to think about backup strategies, security, scalability, and the ease of deployment and maintenance.

## Cluster Architecture

This project uses a GitOps approach to manage the infrastructure and applications deployed on my Kubernetes cluster. The project structure is organized as follows:

<table>
    <tr>
        <th>Directory</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>apps</td>
        <td>Contains all applications deployed on the cluster, organized by environment</td>
    </tr>
    <tr>
        <td>clusters</td>
        <td>Specific configuration to each cluster</td>
    </tr>
    <tr>
        <td>docs</td>
        <td>Project documentation</td>
    </tr>
    <tr>
        <td>infrastructure</td>
        <td>Infrastructure core components (controllers, configs)</td>
    </tr>
    <tr>
        <td>monitoring</td>
        <td>Monitoring and observability tools</td>
    </tr>
    <tr>
        <td>utils</td>
        <td>Various scripts and utilities</td>
    </tr>
</table>

## :computer: Hardware

The cluster is built with accessible and energy-efficient components, ideal for a home lab environment.

### Nodes

I use mini PCs and virtual machines for my Kubernetes cluster, offering a good balance between performance, cost, and power consumption.

## :rocket: Installed Apps & Tools

### Media Applications

<table>
    <tr>
        <th>Logo</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/plex.svg"></td>
        <td><a href="https://www.plex.tv/">Plex</a></td>
        <td>Media server for organizing and streaming movies, TV shows, music, and photos</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/sonarr.svg"></td>
        <td><a href="https://sonarr.tv/">Sonarr</a></td>
        <td>Smart TV show downloader and manager</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/radarr.svg"></td>
        <td><a href="https://radarr.video/">Radarr</a></td>
        <td>Movie collection manager for Usenet and BitTorrent users</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/jackett.svg"></td>
        <td><a href="https://github.com/Jackett/Jackett">Jackett</a></td>
        <td>API proxy for torrent sites</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/overseerr.svg"></td>
        <td><a href="https://overseerr.dev/">Overseerr</a></td>
        <td>Media request manager for Plex</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/flaresolverr.svg"></td>
        <td><a href="https://github.com/FlareSolverr/FlareSolverr">FlareSolverr</a></td>
        <td>Proxy to bypass Cloudflare protection</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/transmission.svg"></td>
        <td><a href="https://transmissionbt.com/">Transmission</a></td>
        <td>Fast, easy, and free BitTorrent client</td>
    </tr>
    <tr>
        <td><img width="32" src=""></td>
        <td><a href="https://github.com/RatingPosterDB/PlexAniSync">PlexAniSync</a></td>
        <td>Sync your Plex libraries with AniList</td>
    </tr>
    <tr>
        <td><img width="32" src=""></td>
        <td><a href="https://github.com/RemiRigal/Plex-Auto-Languages">PlexAutoLanguages</a></td>
        <td>Automatically sets audio and subtitle tracks in Plex based on user preferences</td>
    </tr>
</table>

### Infrastructure

Everything needed to run my cluster and deploy my applications.

<table>
    <tr>
        <th>Logo</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/flux-cd.svg"></td>
        <td><a href="https://fluxcd.io/">Flux CD</a></td>
        <td>My GitOps solution of choice for continuous deployment</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/prometheus.svg"></td>
        <td><a href="https://prometheus.io/">Prometheus</a></td>
        <td>Monitoring system with dimensional data model and flexible query language</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/svg/grafana.svg"></td>
        <td><a href="https://grafana.com/">Grafana</a></td>
        <td>Open observability platform for metric visualization</td>
    </tr>
    <tr>
        <td><img width="32" src="https://www.svgrepo.com/download/374041/renovate.svg"></td>
        <td><a href="https://github.com/renovatebot/renovate">Renovate</a></td>
        <td>Automated dependency updates</td>
    </tr>
    <tr>
        <td><img width="32" src="https://cdn.jsdelivr.net/gh/walkxcode/dashboard-icons/png/cloudflare-zero-trust.png"></td>
        <td><a href="https://developers.cloudflare.com/cloudflare-one/">Cloudflare</a></td>
        <td>Used for DNS management and traffic protection</td>
    </tr>
    <tr>
        <td><img width="32" src="https://www.svgrepo.com/download/530451/dns.svg"></td>
        <td><a href="https://github.com/kubernetes-sigs/external-dns">External DNS</a></td>
        <td>Synchronizes exposed Kubernetes Services and Ingresses with DNS providers</td>
    </tr>
    <tr>
        <td><img width="32" src="https://www.svgrepo.com/download/477066/lock.svg"></td>
        <td><a href="https://external-secrets.io/latest/">External Secrets Operator</a></td>
        <td>Used to sync secrets from 1Password to my cluster</td>
    </tr>
</table>

## Networking

I use Flannel as my CNI (Container Network Interface), which comes as the default network provider with K3s. This provides simple and efficient networking for my Kubernetes cluster.

## Secret Management

I use External Secrets with 1Password to manage secrets in my cluster. This allows me to store sensitive information securely in 1Password and sync them to my cluster. For smaller use cases, I also use SOPS for encrypting secrets directly in Git.

## Storage

I use local storage for my persistent data, leveraging Rancher's local-path provisioner which is the default storage class in K3s. This allows for simple persistent volume management without the need for external storage systems.

## Monitoring and Observability

My monitoring stack includes Prometheus for metrics collection and Grafana for visualization. This allows me to monitor the health of my cluster and the applications deployed on it.

## To Do

- [ ] Migrate to Talos Linux
- [ ] Implement Cilium as CNI
- [ ] Migrate to shared storage with NAS and the iSCSI plugin
- [ ] Implement an automated backup solution for persistent volumes
- [ ] Set up Authentik for authentication
- [ ] Add custom Grafana dashboards for better visualization
- [ ] Set up private runner with Action Runner Controller
- [ ] Implement N8N for workflow automation
- [ ] Deploy KubeShark for network traffic analysis
- [ ] Implement vCluster for multi-tenancy
- [ ] Explore options for high availability

## Useful Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/home/)
- [K3s Documentation](https://docs.k3s.io/)
- [GitOps with Flux CD](https://fluxcd.io/docs/)
- [Self-hosting Guide](https://github.com/awesome-selfhosted/awesome-selfhosted)

---

This project is constantly evolving and serves as a learning platform for the Cloud-Native ecosystem and Kubernetes practices.
