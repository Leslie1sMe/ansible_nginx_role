Nginx
=========

Making the installation of nginx  easily.

Requirements
------------

well, you should use ansible version >=2.4

Role Variables
--------------

the variables i wrote in the vars/main.yml as below:

    
     nginx_host: xxxx.xxx   
     nginx_web_site: "/var/www/html"  
     nginx_port: 80   
     nginx_user: www-data  
     nginx_pid: "/run/nginx.pid"  
     nginx_worker_connections: 768
    

Example
----------------

You can use the role easily by using a brief playbook.yml for example:

    - hosts: servers
      roles:
         - { role: leslie1sme.ansible_nginx_role}
         
         
        
  and just run in the command: ansible-playbook playbook.yml,Do not forget to change the value of the variables,enjoy it :)


License
-------

BSD

Author Information
------------------

github: https://github.com/Leslie1sMe, help me do the things better,thank u guys.
