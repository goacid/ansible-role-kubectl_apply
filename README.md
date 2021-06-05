# Ansible Role - Kubectl Apply

Apply recursly K8S manifests based on exiting dirs

To define in your playbook vars or inventory
 - kubectl_apply_basedir: where the manifest are located

The manifest must contain a file name 'vars' which contain at leat:
- {{ dir }}_deploy_action: "apply" # or "apply"
ex : pihole_deploy_action: "apply" when tree is 
    
    {{ dir_of_playbook }}/manifests/pihole

