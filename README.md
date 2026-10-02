# Hidden-Gem Resources for Cloud, DevOps and SRE

*Under-rated learning resources beyond the usual hands-on lab platforms (iximiuz Labs, KodeKloud, Killercoda, etc.). Compiled October 2, 2026.*

---

## Starting list: hands-on lab platforms

- [iximiuz Labs](https://labs.iximiuz.com/)
- [ADINUSA](https://adinusa.id/)
- [KodeKloud](https://kodekloud.com/)
- [Google Cloud Skills Boost](https://www.skills.google/)
- [Killercoda](https://killercoda.com/)
- [LabEx](https://labex.io/)

The sections below are the hidden gems that go beyond these.

## Troubleshooting and fundamentals

- **[SadServers](https://sadservers.com/)**: gives you a broken Linux/DevOps environment and a problem statement, and you fix it. It's free, runs in the browser, and has community-submitted scenarios, but has no structured path and no explanation after you solve one. It's good prep for live-troubleshooting interviews.
- **[pwn.college](https://pwn.college/)**: an Arizona State University platform that teaches Linux internals through structured challenges. It's useful for understanding the primitives that containers are built on.
- **Grafana Play**: a live public Grafana instance preloaded with dashboards, Loki logs, Prometheus metrics, Tempo traces and alert rules, so you can practice PromQL and LogQL without building a stack.
- **[Play with Kubernetes](https://labs.play-with-k8s.com/) / [Play with Docker](https://training.play-with-docker.com/)**: free browser sandboxes with roughly 4-hour sessions. Play with Kubernetes has you bootstrap a multi-node cluster yourself.
- **[Linux Upskill Challenge](https://linuxupskillchallenge.org/)** and **[OverTheWire Bandit](https://overthewire.org/wargames/bandit/)**: a free 20-day sysadmin course on a real VPS, and an SSH wargame that teaches terminal skills through puzzles.
- **[Learn Git Branching](https://learngitbranching.js.org/)** and **[HashiCorp's Terraform tutorials](https://developer.hashicorp.com/terraform/tutorials)**: a visual puzzle game for rebase and cherry-pick, and official IaC tutorials that start with a local Docker provider.
- **Two angles on platforms you already have:**
  - **[iximiuz](https://labs.iximiuz.com/)**: playgrounds can have up to 5 VMs on custom networks, which suits complex networking scenarios. It also hosts "Kubernetes the (Very) Hard Way", which assembles a cluster with no automation.
  - **[Killercoda](https://killercoda.com/)**: vendors such as Grafana and Cilium publish official tutorials there.

## SRE

- **[Google SRE Classroom](https://sre.google/classroom/)**: workshops from Google's SRE group on non-abstract large systems design, including Distributed PubSub and Distributed ImageServer, plus The Art of SLOs. Many people only read the SRE book and skip this.
- **[The Art of SLOs](https://sre.google/resources/practices-and-processes/art-of-slos/)**: the full materials (slides, a 28-page participant handbook and a facilitator guide) are free under CC BY 4.0. You could run it with a team or at a community meetup.
- **[sre.google resources](https://sre.google/)**: beyond the books, it has Prodverbs, a Measuring Reliability section, and talks such as "Why Heroism is Bad".
- **How They SRE** and **[awesome-sre](https://github.com/dastergon/awesome-sre)**: How They SRE collects public engineering-blog and conference material on how companies run SRE, and awesome-sre is a curated list of SRE resources.
- **Becoming SRE** and **Seeking SRE** (David Blank-Edelman): recommended by Google's Steve McGhee. Becoming SRE is aimed at teams starting out on reliability, and Seeking SRE is a deep dive into the underlying concepts.

## Learning from other people's outages

[k8s.af](https://k8s.af/) is a curated list of public Kubernetes postmortems and failure talks. Entries tag the components involved, such as CoreDNS, CPU throttling, OOMKill, etcd and ELB dynamic IPs. One caveat: many of the entries I could see date from 2017 to 2019, so the root causes are still instructive but the tooling has moved on.

## AWS/EKS-specific

- **[EKS Workshop](https://eksworkshop.com/)**: hands-on modules on fundamentals, autoscaling, observability, security, networking and automation (GitOps). You can pick modules in any combination. It uses one consistent sample retail app and provisions the cluster with Terraform.
- **[EKS Best Practices Guide](https://docs.aws.amazon.com/eks/latest/best-practices/introduction.html)**: day-2 operations guidance published on GitHub, with an open-source CLI called [hardeneks](https://github.com/aws-samples/hardeneks) that checks some of its recommendations against a cluster.
- **Companion guides**: AWS also lists Data on EKS, the AWS observability best practices guide, and EKS Blueprints for Terraform.

## If I had to pick five

SadServers for weekly reps, SRE Classroom for design and SLO thinking, k8s.af for failure patterns, the EKS Best Practices Guide with hardeneks for AWS, and Kubernetes the (Very) Hard Way for internals.

## A note on sources

I haven't tried most of these myself. The hands-on platform details come from a recent roundup and the vendors' own pages, so check free-tier limits before you depend on them.
