common_git-clone-repos

=========

This role will create local folder if not exists and download all the choosen repositories

Requirements
------------

All dependencies will appear on requirements.yml file

Role Variables
--------------
#EXAMPLE how to use it. DON'T UNCOMMENT
git_repos:
   gke:
     repo_name: gke/gke
     repo_project: monolith/
     repo_git_name: "{{ gitlab_git_name }}"
     repo_git_url: "{{ github_git_url }}"
     repo_git_branch: banch
     #for github repos is is repo_user, for bitbucket is repo_team
     repo_git_user: "{{ github_repo_user }}"

true, false
clone_repos: true



Dependencies
------------

All dependencies will appear on requirements.yml file

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - xussof.common_git-clone-repos

License
-------

BSD

Author Information
------------------
Made by @xussof
