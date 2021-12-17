# vault-ssh-agent

## Introduction 

vault-ssh-agent combines dynamic in-memory SSH key generation, Vault SSH CA signing, and an integrated SSH agent to enable secure SSH key management. It is not a replacement for workstation ssh-agent and was designed to be used in transient/ephermeral environments such as CI/CD pipelines or automation platforms. 

vault-ssh-agent is currently being developed but has the following goals:

- Securely generate in-memory SSH keypairs
- Support one or more Vault servers and one or more SSH CA roles to sign keypairs
- Vault Auth Methods: Token/Credential Helper, AppRole, JWT/OIDC, AWS, Azure, GCP, PKI
- SSH agent implementation; can be run as a background daemon.
- HCL2 configuration
- Single static binary
