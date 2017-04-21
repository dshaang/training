# OCDF交付运维人员培训计划
## 目录
1. OCDF(Openshift、Kubernetes)关键要素  
	* Openshift Master（ApiServer、Controller）     
	* Openshift Node  
	* POD
	* Label
	* Service
	* ReplicationController
	* DeploymentConfig
	* BuildConfig
	* PersistentVolume
	* PersittentVolumeClaim
	* ConfigMap
	* Secrets
	* DeamonSet
	* ServiceBroker
	* BackingService
	* BackingServiceInstance
1. 集群容量规划与安装 [https://docs.openshift.org/1.2/install_config/install/index.html](https://docs.openshift.org/1.2/install_config/install/index.html)
	* Openshift容量规划（IP地址、镜像存储、容器存储）
	* Openshift准备安装环境（主机ssh互信、Dockers Registry、Yum Repo、DNS、安装依赖工具包）  
	[https://docs.openshift.org/1.2/install_config/install/prerequisites.html](https://docs.openshift.org/1.2/install_config/install/prerequisites.html)
	* 安装Dockers及设置Docker存储   
	[https://docs.openshift.org/1.2/install_config/install/prerequisites.html#configuring-docker-storage](https://docs.openshift.org/1.2/install_config/install/prerequisites.html#configuring-docker-storage)
	* Openshift准备安装脚本   
	[https://docs.openshift.org/1.2/install_config/install/advanced_install.html](https://docs.openshift.org/1.2/install_config/install/advanced_install.html)
	* Openshift安装与反安装   
	[https://docs.openshift.org/1.2/install_config/install/advanced_install.html#uninstalling-advanced](https://docs.openshift.org/1.2/install_config/install/advanced_install.html#uninstalling-advanced)
	* Openshift常用安装参数说明   
	[https://github.com/openshift/openshift-ansible/blob/master/inventory/byo/hosts.origin.example](https://github.com/openshift/openshift-ansible/blob/master/inventory/byo/hosts.origin.example)
	* 部署OCDF服务及ServiceBroker服务
1. 管理及配置OCDF集群  
	* master-config.yaml说明   
	[https://docs.openshift.org/1.2/install_config/master_node_configuration.html#master-configuration-files](https://docs.openshift.org/1.2/install_config/master_node_configuration.html#master-configuration-files)
	* 授权   
	[https://docs.openshift.org/1.2/install_config/configuring_authentication.html](https://docs.openshift.org/1.2/install_config/configuring_authentication.html)
    [https://docs.openshift.org/1.2/admin_guide/manage_authorization_policy.html](https://docs.openshift.org/1.2/admin_guide/manage_authorization_policy.html)
	* 安全   
	[https://docs.openshift.org/1.2/install_config/configuring_authentication.html](https://docs.openshift.org/1.2/install_config/configuring_authentication.html)  
	[https://docs.openshift.org/1.2/admin_guide/manage_scc.html](https://docs.openshift.org/1.2/admin_guide/manage_scc.html)  
	* 内建镜像仓库    
	[https://docs.openshift.org/1.2/install_config/install/docker_registry.html](https://docs.openshift.org/1.2/install_config/install/docker_registry.html)
	* Router    
	[https://docs.openshift.org/1.2/install_config/install/deploy_router.html](https://docs.openshift.org/1.2/install_config/install/deploy_router.html)
	* 备份及恢复   
	[https://docs.openshift.org/1.2/admin_guide/backup_restore.html](https://docs.openshift.org/1.2/admin_guide/backup_restore.html)
	* 历史数据清理     
	[https://docs.openshift.org/1.2/admin_guide/pruning_resources.html](https://docs.openshift.org/1.2/admin_guide/pruning_resources.html)
	* 增加Openshift Master   
	[https://docs.openshift.org/1.2/install_config/adding_hosts_to_existing_cluster.html#adding-nodes-advanced](https://docs.openshift.org/1.2/install_config/adding_hosts_to_existing_cluster.html#adding-nodes-advanced)
	* 增加Openshift Node   
	[https://docs.openshift.org/1.2/install_config/adding_hosts_to_existing_cluster.html#adding-nodes-advanced](https://docs.openshift.org/1.2/install_config/adding_hosts_to_existing_cluster.html#adding-nodes-advanced)
1. 管理及配置OCDF节点
	* node-config.yaml说明   
	[https://docs.openshift.org/1.2/install_config/master_node_configuration.html#node-configuration-files](https://docs.openshift.org/1.2/install_config/master_node_configuration.html#node-configuration-files)
	* 单节点重启操作流程   
		1.  设置单节点禁止调度   
		[https://docs.openshift.org/1.2/admin_guide/manage_nodes.html#marking-nodes-as-unschedulable-or-schedulable](https://docs.openshift.org/1.2/admin_guide/manage_nodes.html#marking-nodes-as-unschedulable-or-schedulable)   
   		1. 清理节点运行容器    
   		[https://docs.openshift.org/1.2/admin_guide/manage_nodes.html#evacuating-pods-on-nodes](https://docs.openshift.org/1.2/admin_guide/manage_nodes.html#evacuating-pods-on-nodes)
	* 节点配额    
	[https://docs.openshift.org/1.2/admin_guide/allocating_node_resources.html](https://docs.openshift.org/1.2/admin_guide/allocating_node_resources.html)
1. 管理及配置OCDF项目     
	* 项目初始化模板     
	[https://docs.openshift.org/1.2/admin_guide/managing_projects.html#modifying-the-template-for-new-projects](https://docs.openshift.org/1.2/admin_guide/managing_projects.html#modifying-the-template-for-new-projects)
	* 项目配额  
	[https://docs.openshift.org/1.2/admin_guide/quota.html](https://docs.openshift.org/1.2/admin_guide/quota.html)
    [https://docs.openshift.org/1.2/admin_guide/limits.html](https://docs.openshift.org/1.2/admin_guide/limits.html)
    [https://docs.openshift.org/1.2/dev_guide/compute_resources.html](https://docs.openshift.org/1.2/dev_guide/compute_resources.html)
	* 授权   
	[https://github.com/openshift/training/blob/master/03-Auth-Projects-and-Web-Console.md](https://github.com/openshift/training/blob/master/03-Auth-Projects-and-Web-Console.md) 
	* 项目级调度规则  
	[https://docs.openshift.org/1.2/admin_guide/managing_projects.html#using-node-selectors](https://docs.openshift.org/1.2/admin_guide/managing_projects.html#using-node-selectors)
	* 管理Dc  
	[https://docs.openshift.org/1.2/dev_guide/deployments.html](https://docs.openshift.org/1.2/dev_guide/deployments.html)
	* 管理Bc  
	[https://docs.openshift.org/1.2/dev_guide/builds.html](https://docs.openshift.org/1.2/dev_guide/builds.html)
	* 管理持久化卷  
	[https://docs.openshift.org/1.2/dev_guide/volumes.html](https://docs.openshift.org/1.2/dev_guide/volumes.html)   
	[https://docs.openshift.org/1.2/dev_guide/persistent_volumes.html](https://docs.openshift.org/1.2/dev_guide/persistent_volumes.html)  

	* 管理ConfigMap/Secrets
	[https://docs.openshift.org/1.2/dev_guide/secrets.html](https://docs.openshift.org/1.2/dev_guide/secrets.html)
    [https://docs.openshift.org/1.2/dev_guide/configmaps.html](https://docs.openshift.org/1.2/dev_guide/configmaps.html)
	* 管理DeamonSet  
	[https://docs.openshift.org/1.2/dev_guide/daemonsets.html](https://docs.openshift.org/1.2/dev_guide/daemonsets.html)
	* 登录容器  
	[https://docs.openshift.org/1.2/dev_guide/ssh_environment.html](https://docs.openshift.org/1.2/dev_guide/ssh_environment.html)
	[https://docs.openshift.org/1.2/dev_guide/executing_remote_commands.html](https://docs.openshift.org/1.2/dev_guide/executing_remote_commands.html)
    [https://docs.openshift.org/1.2/dev_guide/copy_files_to_container.html](https://docs.openshift.org/1.2/dev_guide/copy_files_to_container.html)
 	* 事件及日志  
 	[https://docs.openshift.org/1.2/dev_guide/events.html](https://docs.openshift.org/1.2/dev_guide/events.html)
