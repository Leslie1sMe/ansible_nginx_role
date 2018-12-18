Nginx
=========

Making the installation of nginx  easily.

Requirements
------------

well, you should use the ansible version >=2.4

Role Variables
--------------

the variables i wrote in the vars/main.yml as below:

    
     nginx_host: xxxx.xxx   //站点域名
     nginx_web_site: "/var/www/html" //站点根目录  
     nginx_port: 80    //站点端口号
     nginx_user: www-data   //nginx的主用户
     nginx_pid: "/run/nginx.pid"    //nginx的pid
     nginx_worker_connections: 768   //nginx进程连接数
    

Example
----------------

You can use the role easily by using a brief playbook.yml for example:

    - hosts: servers
      roles:
         - { role: leslie1sme.ansible_nginx_role}
         
         
        
  run in the command: ansible-playbook playbook.yml,Do not forget to change the value of the variables,enjoy it :)


License
-------

BSD

Author Information
------------------
 
 Help me do it better,thank u guys.

                                                    
                                                     Leslie