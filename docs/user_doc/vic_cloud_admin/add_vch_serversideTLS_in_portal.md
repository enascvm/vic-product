# Add Container Hosts with Server-Side TLS Authentication #

If a Docker host or a vSphere Integrated Containers virtual container host (VCH) implements server-side authentication without verification of client certificates, you do not provide a certificate when you add the host to a project in the management portal. Connections to the host use HTTPS.

**IMPORTANT**: You should only register a VCH with one project at a time. Similarly, you should not add the same VCH to projects in multiple instances of vSphere Integrated Containers.

**Prerequisite**

Log in to vSphere Integrated Containers Management Portal with a vSphere administrator or Management Portal administrator account. For information about logging in to vSphere Integrated Containers Management Portal, see [Logging In to the Management Portal](logging_in_mp.md).

**Procedure**

1. In the **Home** view, click the **Project**  drop-down menu and select the project to which to add the host.
2. Navigate to **Infrastructure** > **Container Hosts** and click **+Host**.
2. On the New Container Host page, configure the host settings.
	1. Enter name for the host.
	2. Select **VCH** or **Docker** as type.
	2. Enter the endpoint for the VCH as URL.

	    For example, *https://*hostname*:2376*.
	
	3. Do not enter credentials and click **Save**. 
	4. If you are prompted to trust the  certificate, click **OK**.

**Result**

The host appears on the Container Hosts page for the selected project. You can also see the host that you added to a project by navigating to **Administration** > **Projects** > *project* > **Infrastructure**.

**What to Do Next**

[Configure Project Settings](manage_projects.md)