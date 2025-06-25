# accounts_local role

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Please see the collection main page for a higher level description.

## Configuration

Below are the role default values from defaults/main.yml:

<pre>
---
# Enable or disable built-in Administrator
accounts_local_administrator_enable: true

# Enable or disable Ansible user password expiration
accounts_local_ansible_user_password_expires: false

# Show or hide Ansible user on Welcome Screen
accounts_local_ansible_user_show_on_welcome: false


# List of user profiles to delete
# NB. Removes all matching profiles
accounts_local_profiles_delete:
#  - testuser
#  - S-1-5-21-...-1000

# List of local users to delete
accounts_local_users_delete:
#  - testuser

# List of local groups to delete
accounts_local_groups_delete:
#  - testgroup

# List of local groups to create
# Mandatory parameters: name
accounts_local_groups_create:
#  - name: testgroup
#    description: Test Group

# List of local users to create
# Mandatory parameters: name
# All users should be added to Users
accounts_local_users_create:
#  - name: testuser
#    fullname: Test User
#    description: User for testing
#    password: Foobar_12
#    password_expired: false
#    password_never_expires: true
#    user_cannot_change_password: false
#    groups_action: add
#    groups:
#      - Users
#    account_disabled: false
#    account_expires: never
#    account_locked: false
#    login_script: C:\Users\login.ps1
#    home_directory: C:\Users\testuser

# Value for no_log parameter when setting passwords
accounts_local_no_log: true

# List of local group memberships to configure
# Mandatory parameters: name, members, state
# Set state to pure to make membership explicit
accounts_local_group_members:
#  - name: testgroup
#    members:
#      - testuser
#    state: pure

# List of local rights settings to configure
# Mandatory parameters: name, users, action
accounts_local_users_rights:
#  - name: SeCreateSymbolicLinkPrivilege
#    users:
#      - testuser
#    action: remove

# List of user profiles to create
# Mandatory parameters: username
accounts_local_profiles_create:
#  - username: testuser
#    name: test-testuser
</pre>

## License

GPLv3+
