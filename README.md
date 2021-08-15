# GCP-website
Setup Wordpress on GCP using Terraform and  Kubernetes manifests.

<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="Objective_Setup_Wordpress_on_GCP_using_Terraform_and_Kubernetes_manifests_0"></a>Objective: Setup Wordpress on GCP using Terraform and Kubernetes manifests.</h1>
<h3 class="code-line" data-line-start=2 data-line-end=3 ><a id="Description_2"></a>Description:</h3>
<p class="has-line-data" data-line-start="3" data-line-end="6">a. Containerized using Kubernetes<br>
b. Scalable database architecture is deployed<br>
c. A load balancer is used</p>
<h3 class="code-line" data-line-start=7 data-line-end=8 ><a id="Files_7"></a>Files:</h3>
<ul>
<li class="has-line-data" data-line-start="9" data-line-end="10"><a href="http://provider.tf">provider.tf</a> --&gt; The Google provider file</li>
<li class="has-line-data" data-line-start="10" data-line-end="11"><a href="http://varaible.tf">varaible.tf</a> --&gt; To specify the variables</li>
<li class="has-line-data" data-line-start="11" data-line-end="12"><a href="http://vpc.tf">vpc.tf</a> --&gt; Creating a VPC and subnet</li>
<li class="has-line-data" data-line-start="12" data-line-end="13"><a href="http://firewall.tf">firewall.tf</a> --&gt; Adding firewall rule to the created vpc</li>
<li class="has-line-data" data-line-start="13" data-line-end="14"><a href="http://mysql.tf">mysql.tf</a> --&gt; For creating an MYSQL database</li>
<li class="has-line-data" data-line-start="14" data-line-end="15"><a href="http://instance.tf">instance.tf</a> --&gt; To create an Instance named “Project”</li>
<li class="has-line-data" data-line-start="15" data-line-end="16"><a href="http://k8s.tf">k8s.tf</a> --&gt; Creating a Kubernetes cluster in the vpc</li>
<li class="has-line-data" data-line-start="16" data-line-end="17"><a href="http://kube-provider.tf">kube-provider.tf</a> --&gt; Kubernetes provider and connect with the created cluster, creating a deployment using WordPress docker image.</li>
<li class="has-line-data" data-line-start="17" data-line-end="18"><a href="http://load-balancer.tf">load-balancer.tf</a> --&gt; LoadBalancer service of Kubernetes, it will create an external Load Balancer using the Load balancing service provided by GCP.</li>
</ul>
<h3 class="code-line" data-line-start=20 data-line-end=21 ><a id="Output_of_the_task_20"></a>Output of the task:</h3>
<p class="has-line-data" data-line-start="22" data-line-end="26"><strong>GCP</strong><br>
<img src="screenshots/gcp/instances.png" alt="The Instances"><br>
<img src="screenshots/gcp/K8s-cluster.png" alt="The Kubernetes cluster"><br>
<img src="screenshots/gcp/mysql.png" alt="The MySQL Database"></p>
<p class="has-line-data" data-line-start="27" data-line-end="33"><strong>Terraform</strong><br>
<img src="screenshots/Terraform/Infra_Creation01.png" alt="1"><br>
<img src="screenshots/Terraform/Infra_Creation02.png" alt="2"><br>
<img src="screenshots/Terraform/Infra_Creation03.png" alt="3"><br>
<img src="screenshots/Terraform/Infra_Creation04.png" alt="4"><br>
<img src="screenshots/Terraform/ReplicaSet.png" alt="ReplicaSet"></p>
<p class="has-line-data" data-line-start="34" data-line-end="35"><strong>Wordpress</strong></p>
<p class="has-line-data" data-line-start="36" data-line-end="39"><img src="screenshots/wordpress/Welcome_page.png" alt="Wordpress Welcome Page"><br>
<img src="screenshots/wordpress/Wp_setup.png" alt="Wordpress Setup"><br>
<img src="screenshots/wordpress/My_wordpress_website.png" alt="My Wordpress Website"></p>
