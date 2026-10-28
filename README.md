<a id="top"></a>

<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0A2540,100:0078D4&height=210&section=header&text=Isaiah%20%22Zay%22%20Herard&fontSize=46&fontColor=ffffff&animation=fadeIn&desc=Identity%20and%20Privileged%20Access%20Engineering&descAlignY=66&descSize=18)

[![Typing](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&color=0078D4&center=true&vCenter=true&width=720&lines=I+build+identity+systems+in+live+tenants.;Then+I+break+them+on+purpose.;Okta+%2B+Entra+ID+%2B+PIM+%2B+Active+Directory;PAM+Forensic+Analyst+%7C+SC-300+%7C+SC-500+%7C+PMP)](https://github.com/ZayLinux26/iam-analyst-portfolio)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-isaiah--herard-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/isaiah-herard)
[![Email](https://img.shields.io/badge/Email-isaiahherard26%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:isaiahherard26@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-IAM_Analyst_Portfolio-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ZayLinux26/iam-analyst-portfolio)
![Profile views](https://komarev.com/ghpvc/?username=ZayLinux26&style=for-the-badge&color=0078D4&label=Profile+views)

</div>

---

## About me

I'm an identity and privileged access engineer in Chicago, starting as a **PAM Forensic Analyst** in November 2026 and building toward CyberArk PAM engineering.

I came to identity through audit. At Giesecke+Devrient I tested logical access controls for PCI-DSS and ISO 27001. At LOG(N) Pacific I worked IAM and PAM engagements on the other side of that table. So I build the way an auditor would check: every control I set up comes with the evidence that proves it works, and every failure gets written down.

This profile is where that work lives. Everything here runs in a real Entra tenant, a real Okta org, and real Active Directory domain controllers.

<div align="center">

[![Projects shipped](https://img.shields.io/badge/Projects_shipped-16-2EA043?style=for-the-badge)](https://github.com/ZayLinux26/iam-analyst-portfolio)
[![Identity providers](https://img.shields.io/badge/Identity_providers_integrated-4-007DC1?style=for-the-badge&logo=okta&logoColor=white)](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric)
[![Leaver cutoff](https://img.shields.io/badge/Okta_to_Entra_leaver_cutoff-~10_seconds-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric)
[![Users provisioned](https://img.shields.io/badge/Users_provisioned_in_one_run-500-6E40C9?style=for-the-badge&logo=powershell&logoColor=white)](https://github.com/ZayLinux26/entra-bulk-provisioning-engine)

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

<a href="https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=meridian-okta-entra-identity-fabric&theme=tokyonight&hide_border=true" alt="meridian-okta-entra-identity-fabric" /></a>
<a href="https://github.com/ZayLinux26/meridian-okta-ad-lifecycle"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=meridian-okta-ad-lifecycle&theme=tokyonight&hide_border=true" alt="meridian-okta-ad-lifecycle" /></a>
<a href="https://github.com/ZayLinux26/iam-role-mining-engine"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=iam-role-mining-engine&theme=tokyonight&hide_border=true" alt="iam-role-mining-engine" /></a>
<a href="https://github.com/ZayLinux26/aks-pim-jit-access"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=aks-pim-jit-access&theme=tokyonight&hide_border=true" alt="aks-pim-jit-access" /></a>
<a href="https://github.com/ZayLinux26/meridian-jml-engine"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=meridian-jml-engine&theme=tokyonight&hide_border=true" alt="meridian-jml-engine" /></a>
<a href="https://github.com/ZayLinux26/entra-phishing-resistant-mfa"><img src="https://github-readme-stats.vercel.app/api/pin/?username=ZayLinux26&repo=entra-phishing-resistant-mfa&theme=tokyonight&hide_border=true" alt="entra-phishing-resistant-mfa" /></a>

</div>

| Project | What it proves |
|---|---|
| [**meridian-okta-entra-identity-fabric**](https://github.com/ZayLinux26/meridian-okta-entra-identity-fabric) | Okta federated into Entra over SAML, Okta to Entra provisioning, JIT admin with PIM, and a timed outage drill |
| [**meridian-okta-ad-lifecycle**](https://github.com/ZayLinux26/meridian-okta-ad-lifecycle) | Okta's import let a terminated user stay active. My fix contains a leaver in Okta in 1.3 seconds. |
| [**iam-role-mining-engine**](https://github.com/ZayLinux26/iam-role-mining-engine) | Mined roles from 1,000 synthetic identities. Role discovery F1 0.923, SoD detection 1.0 precision and recall. |
| [**aks-pim-jit-access**](https://github.com/ZayLinux26/aks-pim-jit-access) | No standing cluster-admin on Kubernetes. One hour of access with MFA, approval, and a ticket. |
| [**meridian-jml-engine**](https://github.com/ZayLinux26/meridian-jml-engine) | An HR feed drives joiner, mover, and leaver changes into AD and Entra, with containment first |
| [**entra-phishing-resistant-mfa**](https://github.com/ZayLinux26/entra-phishing-resistant-mfa) | Passkeys and Windows Hello enforced through a custom authentication strength, tested against real sign-ins |

[![See all projects](https://img.shields.io/badge/See_all_projects-iam--analyst--portfolio-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ZayLinux26/iam-analyst-portfolio)

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
| A Global Administrator can still show "Unauthorized" on an Azure subscription. Entra roles and Azure RBAC are separate planes. | [Azure custom RBAC](https://github.com/ZayLinux26/iam-analyst-portfolio) |

---

## Skills

**Proven in my public repos**

![Microsoft Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Entra PIM](https://img.shields.io/badge/Entra_PIM-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Conditional Access](https://img.shields.io/badge/Conditional_Access-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Okta](https://img.shields.io/badge/Okta-007DC1?style=for-the-badge&logo=okta&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active_Directory-003366?style=for-the-badge&logo=windows&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white)
![SAML and OIDC](https://img.shields.io/badge/SAML_2.0_and_OIDC-F7931E?style=for-the-badge&logo=openid&logoColor=white)
![Azure RBAC](https://img.shields.io/badge/Azure_RBAC-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Key Vault](https://img.shields.io/badge/Azure_Key_Vault-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AKS](https://img.shields.io/badge/AKS-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![KQL](https://img.shields.io/badge/Log_Analytics_and_KQL-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell_7_and_Graph-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Python](https://img.shields.io/badge/Python_and_pandas-3776AB?style=for-the-badge&logo=python&logoColor=white)
![RHEL](https://img.shields.io/badge/RHEL_and_Podman-EE0000?style=for-the-badge&logo=redhat&logoColor=white)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=for-the-badge&logo=cloudflareworkers&logoColor=white)

**Studying now**

![CyberArk](https://img.shields.io/badge/CyberArk_PAM-6C3C9D?style=for-the-badge)
![Cisco](https://img.shields.io/badge/Cisco_networking-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![OpenShift](https://img.shields.io/badge/OpenShift-EE0000?style=for-the-badge&logo=redhatopenshift&logoColor=white)

**Controls I map every project to**

![NIST](https://img.shields.io/badge/NIST_SP_800--53-003366?style=for-the-badge)
![HIPAA](https://img.shields.io/badge/HIPAA-0066CC?style=for-the-badge)
![PCI-DSS](https://img.shields.io/badge/PCI--DSS_v4.0-1A1A1A?style=for-the-badge)
![SOX](https://img.shields.io/badge/SOX_ITGC-4B0082?style=for-the-badge)
![ISO 27001](https://img.shields.io/badge/ISO_27001-005EB8?style=for-the-badge)

---

## Certifications

**Earned**

![Security+](https://img.shields.io/badge/CompTIA-Security%2B-C8202F?style=for-the-badge&logo=comptia&logoColor=white)
![PMP](https://img.shields.io/badge/PMI-PMP-005A9C?style=for-the-badge)
![SC-500](https://img.shields.io/badge/Microsoft-SC--500-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![SC-300](https://img.shields.io/badge/Microsoft-SC--300-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![AZ-104](https://img.shields.io/badge/Microsoft-AZ--104-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![AZ-900](https://img.shields.io/badge/Microsoft-AZ--900-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![GFACT](https://img.shields.io/badge/GIAC-GFACT-004088?style=for-the-badge)
![OCI Foundations](https://img.shields.io/badge/Oracle-OCI_Foundations-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Oracle Autonomous DB](https://img.shields.io/badge/Oracle-Autonomous_DB_Professional-F80000?style=for-the-badge&logo=oracle&logoColor=white)

**Next, in order**

![1](https://img.shields.io/badge/1-CyberArk_Defender-6C3C9D?style=for-the-badge)
![2](https://img.shields.io/badge/2-CyberArk_Sentry-6C3C9D?style=for-the-badge)
![3](https://img.shields.io/badge/3-CCNA-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![4](https://img.shields.io/badge/4-RHCSA-EE0000?style=for-the-badge&logo=redhat&logoColor=white)
![5](https://img.shields.io/badge/5-RHCE-EE0000?style=for-the-badge&logo=redhat&logoColor=white)
![6](https://img.shields.io/badge/6-OpenShift_Administrator-EE0000?style=for-the-badge&logo=redhatopenshift&logoColor=white)

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

[![Connect on LinkedIn](https://img.shields.io/badge/Connect_on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/isaiah-herard)
[![Email me](https://img.shields.io/badge/Email-isaiahherard26%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:isaiahherard26@gmail.com)
[![Portfolio](https://img.shields.io/badge/Browse_the-Portfolio-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ZayLinux26/iam-analyst-portfolio)

If something here helped you, star the repo. It helps other people find it too.

[![Back to top](https://img.shields.io/badge/Back_to_top-555555?style=for-the-badge&logo=github&logoColor=white)](#top)

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:0078D4,100:0A2540&height=120&section=footer)

</div>
