# ansible-tuned

#### start profile
Run the playbook to install tuned on all the hosts mentioned under tuned group in inventory and start a profile
$ ansible-playbook --extra-vars '{ "PROFILE":" " }' tuned.yml

#### Disable all the running profiles
$ ansible-playbook --extra-vars '{ "DISABLE":"yes" }' tuned.yml

#### Recommend a profile and start it 
$ ansible-playbook --extra-vars '{ "RECOMMEND":"yes" }' tuned.yml

#### start your own profile
$ ansible-playbook --extra-vars '{ "PROFILE_NAME":"name-of-the profile", "PROFILE_PATH": "path-to-your-profile" }' tuned.yml
