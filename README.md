<a id="top"></a>

<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0A2540,100:0078D4&height=210&section=header&text=Isaiah%20%22Zay%22%20Herard&fontSize=46&fontColor=ffffff&animation=fadeIn&desc=Identity%20and%20Privileged%20Access%20Engineering&descAlignY=66&descSize=18)

[![Typing](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&color=0078D4&center=true&vCenter=true&width=720&lines=I+build+identity+systems+in+live+tenants.;Then+I+break+them+on+purpose.;Okta+%2B+Entra+ID+%2B+PIM+%2B+Active+Directory;PAM+Forensic+Analyst+%7C+SC-300+%7C+SC-500+%7C+PMP)](https://github.com/ZayLinux26/iam-analyst-portfolio)

[![LinkedIn](./assets/badges/linkedin.svg)](https://www.linkedin.com/in/isaiah-herard)
[![Email](./assets/badges/email.svg)](mailto:isaiahherard26@gmail.com)
[![Portfolio](./assets/badges/portfolio.svg)](https://github.com/ZayLinux26/iam-analyst-portfolio)
![Profile views](https://komarev.com/ghpvc/?username=ZayLinux26&style=for-the-badge&color=0078D4&label=Profile+views)

</div>

---

## About me

I'm an identity and privileged access engineer in Chicago, starting as a **PAM Forensic Analyst** in November 2026 and building toward CyberArk PAM engineering.

I came to identity through audit. At Giesecke+Devrient I tested logical access controls for PCI-DSS and ISO 27001. At LOG(N) Pacific I worked IAM and PAM engagements on the other side of that table. So I build the way an auditor would check: every control I set up comes with the evidence that proves it works, and every failure gets written down.

This profile is where that work lives. Everything here runs in a real Entra tenant, a real Okta org, and real Active Directory domain controllers.

<div align="center">

[![Projects shipped](./assets/badges/projects-shipped.svg)](https://github.com/ZayLinux26/iam-analyst-portfolio)
[![Identity providers](./assets/badges/identity-providers.svg)](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric)
[![Leaver cutoff](./assets/badges/leaver-cutoff.svg)](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric)
[![Users provisioned](./assets/badges/users-provisioned.svg)](https://github.com/ZayLinux26/entra-bulk-provisioning-engine)

</div>

---

## Start here

### [Meridian Identity Fabric: Okta + Entra ID Federation with JIT Privileged Access](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric)

My capstone. Active Directory owns the person, Okta signs them in, and Entra trusts Okta over SAML 2.0. Admin rights in Entra come only from a time-boxed PIM activation with a ticket number.

- **One AD disable cuts someone off everywhere.** Okta deactivated the user, and Entra disabled the account about 10 seconds later.
- **Okta's MFA unlocks Entra admin roles.** A federated user activated a PIM role with a phishing-resistant passkey from Okta.
- **I took Okta down on purpose.** Federated users were locked out, both cloud-only admin paths still worked, and recovery took 10 minutes.
- **13 things broke along the way,** and the README documents every one. The hardest needed an Okta inline hook I wrote and ran on Cloudflare Workers.

---

## Featured work

<div align="center">

<a href="https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric"><img src="./assets/cards/meridian-okta-entra-identity-fabric.svg" alt="meridian-okta-entra-identity-fabric" width="415" /></a>
<a href="https://github.com/ZayLinux26/meridian-okta-ad-lifecycle"><img src="./assets/cards/meridian-okta-ad-lifecycle.svg" alt="meridian-okta-ad-lifecycle" width="415" /></a>
<a href="https://github.com/ZayLinux26/iam-role-mining-engine"><img src="./assets/cards/iam-role-mining-engine.svg" alt="iam-role-mining-engine" width="415" /></a>
<a href="https://github.com/ZayLinux26/aks-pim-jit-access"><img src="./assets/cards/aks-pim-jit-access.svg" alt="aks-pim-jit-access" width="415" /></a>
<a href="https://github.com/ZayLinux26/meridian-jml-engine"><img src="./assets/cards/meridian-jml-engine.svg" alt="meridian-jml-engine" width="415" /></a>
<a href="https://github.com/ZayLinux26/entra-phishing-resistant-mfa"><img src="./assets/cards/entra-phishing-resistant-mfa.svg" alt="entra-phishing-resistant-mfa" width="415" /></a>

</div>

| Project | What it proves |
|---|---|
| [**meridian-okta-entra-identity-fabric**](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric) | Okta federated into Entra over SAML, Okta to Entra provisioning, JIT admin with PIM, and a timed outage drill |
| [**meridian-okta-ad-lifecycle**](https://github.com/ZayLinux26/meridian-okta-ad-lifecycle) | Okta's import let a terminated user stay active. My fix contains a leaver in Okta in 1.3 seconds. |
| [**iam-role-mining-engine**](https://github.com/ZayLinux26/iam-role-mining-engine) | Mined roles from 1,000 synthetic identities. Role discovery F1 0.923, SoD detection 1.0 precision and recall. |
| [**aks-pim-jit-access**](https://github.com/ZayLinux26/aks-pim-jit-access) | No standing cluster-admin on Kubernetes. One hour of access with MFA, approval, and a ticket. |
| [**meridian-jml-engine**](https://github.com/ZayLinux26/meridian-jml-engine) | An HR feed drives joiner, mover, and leaver changes into AD and Entra, with containment first |
| [**entra-phishing-resistant-mfa**](https://github.com/ZayLinux26/entra-phishing-resistant-mfa) | Passkeys and Windows Hello enforced through a custom authentication strength, tested against real sign-ins |

[![See all projects](./assets/badges/see-all-projects.svg)](https://github.com/ZayLinux26/iam-analyst-portfolio)

---

## Field notes

Things I found by building, that the vendor docs don't put up front.

| What I found | Where |
|---|---|
| Okta's scheduled AD import never sees a leaver who was moved out of its OU scope. The console only catches up when someone looks the user up. | [okta-ad-lifecycle](https://github.com/ZayLinux26/meridian-okta-ad-lifecycle#finding-1-the-leaver-gap) |
| With delegated auth on, Okta can let a user sign in for up to five days while every AD agent is down. AD isn't asked at all. | [okta-ad-lifecycle](https://github.com/ZayLinux26/meridian-okta-ad-lifecycle#finding-2-the-agent-outage-and-the-credential-cache) |
| Over SAML 2.0, Entra ignores an MFA claim sent as an attribute. It only reads `AuthnContextClassRef`, and Okta's UI can't set Microsoft's value there. | [okta-entra-identity-fabric](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric#7-what-broke-and-how-i-fixed-it) |
| Okta's Microsoft 365 connector writes as a directory sync engine, so flipping a user to cloud-managed in Entra blocks Okta from updating them. | [okta-entra-identity-fabric](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric#7-what-broke-and-how-i-fixed-it) |
| Disabling a user doesn't remove their PIM eligibility. The entitlement just sits there until someone reviews it. | [okta-entra-identity-fabric](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric#8-findings) |
| A Global Administrator can still show "Unauthorized" on an Azure subscription. Entra roles and Azure RBAC are separate planes. | [Azure custom RBAC](https://github.com/ZayLinux26/iam-analyst-portfolio#shipped-work) |

---

## Skills

**Proven in my public repos**

![Microsoft Entra ID](./assets/badges/microsoft-entra-id.svg)
![Entra PIM](./assets/badges/entra-pim.svg)
![Conditional Access](./assets/badges/conditional-access.svg)
![Okta](./assets/badges/okta.svg)
![Active Directory](./assets/badges/active-directory.svg)
![Keycloak](./assets/badges/keycloak.svg)
![SAML and OIDC](./assets/badges/saml-and-oidc.svg)
![Azure RBAC](./assets/badges/azure-rbac.svg)
![Key Vault](./assets/badges/key-vault.svg)
![AKS](./assets/badges/aks.svg)
![KQL](./assets/badges/kql.svg)
![PowerShell](./assets/badges/powershell.svg)
![Python](./assets/badges/python.svg)
![RHEL](./assets/badges/rhel.svg)
![Cloudflare Workers](./assets/badges/cloudflare-workers.svg)

**Studying now**

![CyberArk](./assets/badges/cyberark.svg)
![Cisco](./assets/badges/cisco.svg)
![Ansible](./assets/badges/ansible.svg)
![OpenShift](./assets/badges/openshift.svg)

**Controls I map every project to**

![NIST](./assets/badges/nist.svg)
![HIPAA](./assets/badges/hipaa.svg)
![PCI-DSS](./assets/badges/pci-dss.svg)
![SOX](./assets/badges/sox.svg)
![ISO 27001](./assets/badges/iso-27001.svg)

---

## Certifications

**Earned**

![Security+](./assets/badges/security.svg)
![PMP](./assets/badges/pmp.svg)
![SC-500](./assets/badges/sc-500.svg)
![SC-300](./assets/badges/sc-300.svg)
![AZ-104](./assets/badges/az-104.svg)
![AZ-900](./assets/badges/az-900.svg)
![GFACT](./assets/badges/gfact.svg)
![OCI Foundations](./assets/badges/oci-foundations.svg)
![Oracle Autonomous DB](./assets/badges/oracle-autonomous-db.svg)

**Next, in order**

![1](./assets/badges/next-1.svg)
![2](./assets/badges/next-2.svg)
![3](./assets/badges/next-3.svg)
![4](./assets/badges/next-4.svg)
![5](./assets/badges/next-5.svg)
![6](./assets/badges/next-6.svg)

---

## Why identity, PAM, and Linux

```mermaid
flowchart TB
    U(["User or admin"]) --> ID["Identity<br/>Entra ID, Okta, AD<br/>who you are"]
    ID --> PAM["Privileged access<br/>PIM, CyberArk<br/>what you can touch, and for how long"]
    PAM --> INFRA["Infrastructure<br/>Azure, RHEL, Kubernetes<br/>where it actually runs"]
    INFRA -. "audit evidence" .-> AUD["Logs and controls<br/>NIST, HIPAA, PCI, SOX"]
```

Identity is the perimeter. PAM is the safe inside. Linux is the floor the safe sits on. If you can't operate all three together, you can't actually secure the enterprise.

---

## Right now

| | |
|---|---|
| **Starting** | PAM Forensic Analyst, November 2026 |
| **Studying** | CyberArk Defender, then Sentry, both by the end of 2026 |
| **Building** | A SOX and PCI-DSS identity engagement, and Project 10: access reviews scored against a seeded anomaly manifest |
| **Next** | Identity governance for AI agents: an agent registry, delegated OAuth, and auto-revoke when an agent drifts out of policy |

---

## GitHub activity

<div align="center">

![GitHub stats](https://github-readme-stats.vercel.app/api?username=ZayLinux26&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ZayLinux26&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

<div align="center">

## Let's talk

Hiring for identity or privileged access? Working through an Okta, Entra, or PAM problem? Or just following along? I'd like to hear from you.

**Open to:** remote IAM and PAM engineering roles and contracts, identity governance, and roles that sponsor a security clearance.

[![Connect on LinkedIn](./assets/badges/connect-on-linkedin.svg)](https://www.linkedin.com/in/isaiah-herard)
[![Email me](./assets/badges/email.svg)](mailto:isaiahherard26@gmail.com)
[![Portfolio](./assets/badges/portfolio-2.svg)](https://github.com/ZayLinux26/iam-analyst-portfolio)

If something here helped you, star the repo. It helps other people find it too.

[![Back to top](./assets/badges/back-to-top.svg)](#top)

![Footer](./assets/footer.svg)

</div>
