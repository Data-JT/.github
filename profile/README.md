<div align="center">
  <a href="https://www.data-jt.de">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Data-JT/.github/main/profile/banner-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Data-JT/.github/main/profile/banner-light.svg">
      <img alt="Banner showing the logo of Data JT, the company behind these Puppet modules" src="https://raw.githubusercontent.com/Data-JT/.github/main/profile/banner-light.svg" width="100%">
    </picture>
  </a>

  <h3>Proxmox, Greenbone and GLPI, managed as Puppet code.</h3>

  <a href="https://www.data-jt.de">Website</a>&ensp;·&ensp;<a href="https://forge.puppet.com/modules/datajt">Puppet Forge</a>&ensp;·&ensp;<a href="https://www.data-jt.de/kontakt">Contact</a>
</div>

<br>

Data JT is an IT and data protection consultancy near Freiburg, Germany. We publish these Puppet modules on the Puppet Forge under `datajt`, licensed Apache-2.0.

<table>
  <tr><td>
    <a href="https://github.com/Data-JT/puppet-proxmox_virtual_environment"><b>proxmox_virtual_environment</b></a><br>
    <sub>Proxmox Virtual Environment · 21 <code>pve_*</code> types · <a href="https://forge.puppet.com/modules/datajt/proxmox_virtual_environment">Forge</a></sub><br>
    Describe a PVE cluster's storage, backup jobs, users, permissions and SDN in Hiera; Puppet changes only what differs. Writes go through one designated cluster node.
  </td></tr>
  <tr><td>
    <a href="https://github.com/Data-JT/puppet-proxmox_backup_server"><b>proxmox_backup_server</b></a><br>
    <sub>Proxmox Backup Server · 13 <code>pbs_*</code> types · <a href="https://forge.puppet.com/modules/datajt/proxmox_backup_server">Forge</a></sub><br>
    Describe a PBS node's datastores, users, sync, prune and verification jobs in Hiera; Puppet changes only what differs. Remote, LDAP and S3 credentials are drift-checked too.
  </td></tr>
  <tr><td>
    <a href="https://github.com/Data-JT/puppet-proxmox_datacenter_manager"><b>proxmox_datacenter_manager</b></a><br>
    <sub>Proxmox Datacenter Manager · 8 <code>pdm_*</code> types · <a href="https://forge.puppet.com/modules/datajt/proxmox_datacenter_manager">Forge</a></sub><br>
    Describe a PDM instance's remotes, users, permissions and views in Hiera; Puppet changes only what differs.
  </td></tr>
  <tr><td>
    <a href="https://github.com/Data-JT/puppet-greenbone"><b>greenbone</b></a><br>
    <sub>Greenbone Community Edition (OpenVAS) · 12 <code>gvm_*</code> types · <a href="https://forge.puppet.com/modules/datajt/greenbone">Forge</a></sub><br>
    Describe a scanner's schedules, targets, tasks, scan configs and users in Hiera; Puppet changes only what differs. Talks GMP on gvmd's local socket; no UUIDs in the data.
  </td></tr>
  <tr><td>
    <a href="https://github.com/Data-JT/puppet-glpi"><b>glpi</b></a><br>
    <sub>GLPI 11 · 10 <code>glpi_*</code> types · <a href="https://forge.puppet.com/modules/datajt/glpi">Forge</a></sub><br>
    Describe a GLPI instance's rules, clusters, appliances, certificates and locations in Hiera; Puppet changes only what differs. Talks REST API v2 and deletes only objects it marked itself.
  </td></tr>
</table>

All five are native Puppet Resource API types, declared in manifests or from Hiera through one `resources` class. The Proxmox and Greenbone modules never purge undeclared objects, and the three Proxmox modules also detect drift in secrets.

Issues and pull requests go to the respective repository. Everything else: [info@data-jt.de](mailto:info@data-jt.de) or [www.data-jt.de/kontakt](https://www.data-jt.de/kontakt).

<br>

<sub>Data JT UG (haftungsbeschränkt) · <a href="https://www.data-jt.de/impressum">Impressum</a></sub>
