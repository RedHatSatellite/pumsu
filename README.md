This script allows you to build and upload puppet modules into Satellite 6

Example output:
```sh
[root@sat ~]# pumsu -v
20160809

[root@sat ~]# pumsu -o
---|-------------|-------------|------------
ID | NAME        | LABEL       | DESCRIPTION
---|-------------|-------------|------------
3  | LabInternal | LabInternal |            
6  | Test Org    | testOrg     |            
---|-------------|-------------|------------

[root@sat ~]# pumsu -l "Test Org"
---|------|---------|--------------|----
ID | NAME | PRODUCT | CONTENT TYPE | URL
---|------|---------|--------------|----

[root@sat ~]# ./pumsu -l LabInternal
---|----------------|------------------------|--------------|----
ID | NAME           | PRODUCT                | CONTENT TYPE | URL
---|----------------|------------------------|--------------|----
9  | puppet-modules | inhouse-puppet-modules | puppet       |    
---|----------------|------------------------|--------------|----

[root@sat ~]# pumsu --modules module_list.txt --source puppet-modules/ --repoid 9
[*] building module: abrt_ccpp
[*] building module: abrtd
[*] building module: abrt_oops
[*] building module: accts_lock
[*] building module: accts_nologin
[*] building module: atd
[*] building module: auditd
[*] building module: authorized_keys
[*] building module: avahi
[*] building module: chrony
[*] building module: cpumgmt
[*] building module: crond
[*] building module: dbus
[*] building module: device_drivers
[*] building module: dnsmasq
[*] building module: ebtables
[*] building module: extra_facts
[*] building module: filesystems
[*] building module: firewalld
[*] building module: gofer
[*] building module: grub2
[*] building module: haldaemon
[*] building module: hosts
[*] building module: init
[*] building module: ip6tables
[*] building module: iptables
[*] building module: irqbalance
[*] building module: issue
[*] building module: kdump
[*] building module: limits
[*] building module: login_defs
[*] building module: lvm2_lvmetad
[*] building module: lvm2_monitor
[*] building module: mdmonitor
[*] building module: mlocate
[*] building module: motd
[*] building module: netfs
[*] building module: ntp
[*] building module: ntpdate
[*] building module: oddjob
[*] building module: pam_login
[*] building module: password_quality
[*] building module: postfix
[*] building module: profiles
[*] building module: protocols
[*] building module: psacct
[*] building module: puppet
[*] building module: quota_nld
[*] building module: rdisc
[*] building module: restorecond
[*] building module: rhfuncs
[*] building module: rhnsd
[*] building module: rhsmcertd
[*] building module: rsyslog
[*] building module: saslauthd
[*] building module: scheduling
[*] building module: securetty
[*] building module: selinux
[*] building module: shadow
[*] building module: smartd
[*] building module: snmp
[*] building module: sshd
[*] building module: su
[*] building module: sudoers
[*] building module: sysctl
[*] building module: sysstat
[*] building module: tcpwrappers
[*] building module: tuned
[*] building module: udev_rules
[*] building module: useradd_defs
[*] building module: users
[*] building module: xinetd
[*] uploading modules
Successfully uploaded file 'mweetman-abrt_ccpp-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-abrtd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-abrt_oops-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-accts_lock-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-accts_nologin-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-atd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-auditd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-authorized_keys-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-avahi-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-chrony-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-cpumgmt-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-crond-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-dbus-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-device_drivers-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-dnsmasq-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-ebtables-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-extra_facts-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-filesystems-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-firewalld-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-gofer-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-grub2-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-haldaemon-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-hosts-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-init-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-ip6tables-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-iptables-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-irqbalance-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-issue-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-kdump-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-limits-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-login_defs-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-lvm2_lvmetad-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-lvm2_monitor-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-mdmonitor-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-mlocate-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-motd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-netfs-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-ntp-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-ntpdate-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-oddjob-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-pam_login-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-password_quality-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-postfix-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-profiles-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-protocols-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-psacct-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-puppet-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-quota_nld-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-rdisc-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-restorecond-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-rhfuncs-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-rhnsd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-rhsmcertd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-rsyslog-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-saslauthd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-scheduling-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-securetty-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-selinux-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-shadow-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-smartd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-snmp-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-sshd-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-su-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-sudoers-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-sysctl-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-sysstat-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-tcpwrappers-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-tuned-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-udev_rules-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-useradd_defs-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-users-0.1.0.tar.gz'.
Successfully uploaded file 'mweetman-xinetd-0.1.0.tar.gz'.

[*] cleaning up temp dir
[root@sat ~]# hammer repository info --id 9
...
Content Counts:     
    Puppet Modules: 74

```

