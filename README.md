# ansible-gluster-infa
Ansible GlusterFS cluster on Ubuntu at DigitalOcean, using private networking

## Steps:
1. Set your API v1 keys for DO:
export DO_CLIENT_ID=yourID
export DO_API_KEY=yourKey
2. Adjust requested gluster-pool in the "inventory" file in multiples of 2.
3. Adjust the gluster_brick_config replica number (currently 2), depending on if you want a replicate vs distributed replicate.
4. Run ansible-playbook provision.yml.
