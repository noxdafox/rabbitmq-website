<!--
Copyright (c) 2007-2021 VMware, Inc. or its affiliates.

All rights reserved. This program and the accompanying materials
are made available under the terms of the under the Apache License,
Version 2.0 (the "License”); you may not use this file except in compliance
with the License. You may obtain a copy of the License at

https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# Downloading and Installing RabbitMQ

The latest [release](https://github.com/rabbitmq/rabbitmq-server/releases) of RabbitMQ is **&version-server;**. See [change log](changelog.html) for release notes.
See [RabbitMQ support timeline](/versions.html) to find out what release series are supported.

Experimenting with RabbitMQ on your workstation? Try the [community Docker image](https://registry.hub.docker.com/_/rabbitmq/):

<pre class="lang-bash">
# for RabbitMQ 3.9, the latest series
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management
</pre>

<pre class="lang-bash">
# for RabbitMQ 3.8,
# 3.8.x support timeline: https://www.rabbitmq.com/versions.html
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.8-management
</pre>



## Open Source RabbitMQ Server

### Installation Guides

 * Linux, BSD, UNIX: [Debian, Ubuntu](install-debian.html) | [RHEL, CentOS, Fedora](install-rpm.html) | [Generic binary build](install-generic-unix.html) | [Solaris](install-solaris.html)
 * Windows: [Chocolatey or Installer](install-windows.html) (recommended) | [Binary build](install-windows-manual.html)
 * MacOS: [Homebrew](install-homebrew.html) | [Generic binary build](install-generic-unix.html)
 * [Erlang/OTP for RabbitMQ](/which-erlang.html)

### Preview Releases (Betas, Release Candidates)

You can contribute to RabbitMQ by helping the community test preview releases.

Preview releases are [distributed via GitHub](https://github.com/rabbitmq/rabbitmq-server/releases) and marked
as pre-release.

## VMware Tanzu™ RabbitMQ® (Commercial Edition)

 * [Tanzu™ RabbitMQ®](https://tanzu.vmware.com/rabbitmq)
 * [Tanzu™ RabbitMQ® on Kubernetes](kubernetes/tanzu/installation.html)

## Kubernetes

### RabbitMQ Cluster Kubernetes Operator

Open source [RabbitMQ Cluster Kubernetes Operator](kubernetes/operator/operator-overview.html) by VMware (developed [on GitHub](https://github.com/rabbitmq/cluster-operator)):

 * [quickstart guide](kubernetes/operator/quickstart-operator.html)
 * [usage guide](kubernetes/operator/using-operator.html)
 * [OpenShift-specific topics](kubernetes/operator/using-on-openshift.html)
 * [examples](https://github.com/rabbitmq/cluster-operator/tree/main/docs/examples)

### RabbitMQ Topology Kubernetes Operator

Open source [RabbitMQ Topology Kubernetes Operator](kubernetes/operator/using-topology-operator.html) by VMware (developed [on GitHub](https://github.com/rabbitmq/messaging-topology-operator)):

 * [installation guide](kubernetes/operator/install-topology-operator.html)
 * [usage guide](kubernetes/operator/using-topology-operator.html)


Other guides related to Kubernetes:

 * A [peer discovery](/cluster-formation.html) mechanism [for Kubernetes](/cluster-formation.html#peer-discovery-k8s)


## Docker

 * Docker community-maintained [RabbitMQ Docker image](https://registry.hub.docker.com/_/rabbitmq/) ([on GitHub](https://github.com/docker-library/rabbitmq/))


## Cloud

 * [Tanzu™ RabbitMQ®](https://tanzu.vmware.com/rabbitmq)
 * [RabbitMQ Cluster Kubernetes Operator](/kubernetes/operator/install-operator.html) by VMware (developed [on GitHub](https://github.com/rabbitmq/cluster-operator))
 * [Tanzu™ RabbitMQ® on Kubernetes](kubernetes/tanzu/installation.html)
 * [CloudAMQP](https://www.cloudamqp.com): RabbitMQ-as-a-Service available in multiple clouds
 * [Amazon EC2](ec2.html)

## Downloads [on GitHub](https://github.com/rabbitmq/rabbitmq-server/releases)

 * [Windows installer](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-&version-server;.exe)
 * [Debian, Ubuntu](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server_&version-server;-1_all.deb)
 * [RHEL/CentOS 8.x](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-&version-server;-1.el8.noarch.rpm) |
    [RHEL/CentOS 7.x](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-&version-server;-1.el7.noarch.rpm) |
    [OpenSUSE](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-&version-server;-1.suse.noarch.rpm) |
    zero dependency [Erlang 23 RPM](https://github.com/rabbitmq/erlang-rpm)
 * [Generic UNIX binary](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-generic-unix-&version-server;.tar.xz)
 * [Windows binary](https://github.com/rabbitmq/rabbitmq-server/releases/download/v&version-server;/rabbitmq-server-windows-&version-server;.zip)


## Debian (Apt) and RPM (Yum) Repositories

 * [Package Cloud](https://packagecloud.io/rabbitmq/)
 * [Cloudsmith.io](https://cloudsmith.io/~rabbitmq/repos/)

## Provisioning Tools (Chef, Puppet, etc)

 * [Chef cookbook](https://github.com/rabbitmq/chef-cookbook)
 * [Puppet module](https://github.com/puppetlabs/puppetlabs-rabbitmq)


## Release Signing Key

 * [Release Signing Key](https://github.com/rabbitmq/signing-keys/releases/download/2.0/rabbitmq-release-signing-key.asc) <code>0x6B73A36E6026DFCA</code> (on GitHub)
 * [How to Verify Release Artifact Signatures](/signatures.html)
 * [Release Signing Key](/rabbitmq-release-signing-key.asc) (alternative download location on rabbitmq.com)


## Client Libraries

### Java Client

 * On Maven Central: [RabbitMQ Java client](http://search.maven.org/#search%7Cgav%7C1%7Cg%3A%22com.rabbitmq%22%20AND%20a%3A%22amqp-client%22)
 * Quick download: [Maven.org](http://repo1.maven.org/maven2/com/rabbitmq/amqp-client/&version-java-client;/amqp-client-&version-java-client;.jar) |
   [Source](http://repo1.maven.org/maven2/com/rabbitmq/amqp-client/&version-java-client;/amqp-client-&version-java-client;-sources.jar)
 * [API guide](/api-guide.html)
 * [API reference](https://rabbitmq.github.io/rabbitmq-java-client/api/current/) (JavaDoc)
 * [License and other information](/java-client.html)
 * [Older versions](http://repo1.maven.org/maven2/com/rabbitmq/amqp-client/)

### JMS Client

 * On Maven Central: [RabbitMQ JMS Client](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22com.rabbitmq.jms%22%20AND%20a%3A%22rabbitmq-jms%22)

### .NET/C# Client

 * On NuGet: [RabbitMQ .NET Client](https://www.nuget.org/packages/RabbitMQ.Client)
 * [API guide](/dotnet-api-guide.html)
 * [API reference](https://rabbitmq.github.io/rabbitmq-dotnet-client/)
 * [License and other information](/dotnet.html)
 * [Older versions](https://github.com/rabbitmq/rabbitmq-dotnet-client/releases)

### Erlang Client

 * On Hex.pm: [amqp_client](https://hex.pm/packages/amqp_client)

### Clients for Other Languages

The RabbitMQ community has created a large number of [clients and developer tools](devtools.html)
covering a variety of platforms and languages.


## Community Plugins

For your convenience, we offer binary downloads of various
plugins developed by the community.

 * [Description of available plugins](community-plugins.html)

## Snapshot (Alpha) Builds

Snapshot releases of the RabbitMQ broker
available to users who wish to experiment with the latest and
greatest features and bug fixes. For more details, head over to
the [snapshots page](snapshots.html).
