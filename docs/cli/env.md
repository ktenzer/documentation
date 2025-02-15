---
id: env
title: Temporal CLI env command reference
sidebar_label: env
description: How to use the Temporal CLI env command
toc_max_heading_level: 4
---

<!-- THIS FILE IS GENERATED. DO NOT EDIT THIS FILE DIRECTLY -->

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

Environment (or 'env') commands allow the user to configure the properties for the environment in use.

## get

The `temporal env get` command prints the environmental properties for the environment in use.

Use the options listed below to change the command's behavior.
Make sure to write the command as follows:
`temporal env get [command options] [arguments]`

- <a class="tdlp" href="/cli/cmd-options#address">--address<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  address</span><br /><br /><span class="tdlppd">The host and port for the Temporal Frontend Service.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#address">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-auth">--codec-auth<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-auth</span><br /><br /><span class="tdlppd">Sets the authorization header on requests to the Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-auth">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-endpoint">--codec-endpoint<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-endpoint</span><br /><br /><span class="tdlppd">Endpoint for a remote Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-endpoint">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#color">--color<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  color</span><br /><br /><span class="tdlppd">When to use color</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#color">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#context-timeout">--context-timeout<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  context-timeout</span><br /><br /><span class="tdlppd">An optional timeout for the context of an RPC call.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#context-timeout">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#env">--env<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  env</span><br /><br /><span class="tdlppd">Name of the environment to read environmental variables from.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#env">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#grpc-meta">--grpc-meta<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  grpc-meta</span><br /><br /><span class="tdlppd">Contains gRPC metadata to send with requests.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#grpc-meta">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#namespace">--namespace<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  namespace</span><br /><br /><span class="tdlppd">Identifies a Namespace in the Temporal Workflow.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#namespace">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-ca-path">--tls-ca-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-ca-path</span><br /><br /><span class="tdlppd">Path to server CA certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-ca-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-cert-path">--tls-cert-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-cert-path</span><br /><br /><span class="tdlppd">Path to x509 certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-cert-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-disable-host-verification">--tls-disable-host-verification<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-disable-host-verification</span><br /><br /><span class="tdlppd">Disables TLS host name verification if already enabled.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-disable-host-verification">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-key-path">--tls-key-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-key-path</span><br /><br /><span class="tdlppd">Path to private certificate key.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-key-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-server-name">--tls-server-name<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-server-name</span><br /><br /><span class="tdlppd">Provides an override for the target TLS server name.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-server-name">Learn more</a></span></span></a>

## set

The `temporal env set` command sets the value for an environmental property.

Use the options listed below to change the command's behavior.
Make sure to write the command as follows:
`temporal env set [command options] [arguments]`

- <a class="tdlp" href="/cli/cmd-options#address">--address<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  address</span><br /><br /><span class="tdlppd">The host and port for the Temporal Frontend Service.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#address">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-auth">--codec-auth<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-auth</span><br /><br /><span class="tdlppd">Sets the authorization header on requests to the Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-auth">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-endpoint">--codec-endpoint<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-endpoint</span><br /><br /><span class="tdlppd">Endpoint for a remote Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-endpoint">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#color">--color<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  color</span><br /><br /><span class="tdlppd">When to use color</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#color">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#context-timeout">--context-timeout<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  context-timeout</span><br /><br /><span class="tdlppd">An optional timeout for the context of an RPC call.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#context-timeout">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#env">--env<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  env</span><br /><br /><span class="tdlppd">Name of the environment to read environmental variables from.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#env">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#grpc-meta">--grpc-meta<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  grpc-meta</span><br /><br /><span class="tdlppd">Contains gRPC metadata to send with requests.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#grpc-meta">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#namespace">--namespace<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  namespace</span><br /><br /><span class="tdlppd">Identifies a Namespace in the Temporal Workflow.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#namespace">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-ca-path">--tls-ca-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-ca-path</span><br /><br /><span class="tdlppd">Path to server CA certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-ca-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-cert-path">--tls-cert-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-cert-path</span><br /><br /><span class="tdlppd">Path to x509 certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-cert-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-disable-host-verification">--tls-disable-host-verification<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-disable-host-verification</span><br /><br /><span class="tdlppd">Disables TLS host name verification if already enabled.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-disable-host-verification">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-key-path">--tls-key-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-key-path</span><br /><br /><span class="tdlppd">Path to private certificate key.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-key-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-server-name">--tls-server-name<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-server-name</span><br /><br /><span class="tdlppd">Provides an override for the target TLS server name.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-server-name">Learn more</a></span></span></a>

## delete

The `temporal env delete` command deletes a given environment or environmental property.

Use the options listed below to change the command's behavior.
Make sure to write the command as follows:
`temporal env delete [command options]`

- <a class="tdlp" href="/cli/cmd-options#address">--address<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  address</span><br /><br /><span class="tdlppd">The host and port for the Temporal Frontend Service.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#address">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-auth">--codec-auth<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-auth</span><br /><br /><span class="tdlppd">Sets the authorization header on requests to the Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-auth">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#codec-endpoint">--codec-endpoint<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  codec-endpoint</span><br /><br /><span class="tdlppd">Endpoint for a remote Codec Server.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#codec-endpoint">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#color">--color<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  color</span><br /><br /><span class="tdlppd">When to use color</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#color">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#context-timeout">--context-timeout<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  context-timeout</span><br /><br /><span class="tdlppd">An optional timeout for the context of an RPC call.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#context-timeout">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#env">--env<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  env</span><br /><br /><span class="tdlppd">Name of the environment to read environmental variables from.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#env">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#grpc-meta">--grpc-meta<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  grpc-meta</span><br /><br /><span class="tdlppd">Contains gRPC metadata to send with requests.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#grpc-meta">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#namespace">--namespace<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  namespace</span><br /><br /><span class="tdlppd">Identifies a Namespace in the Temporal Workflow.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#namespace">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-ca-path">--tls-ca-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-ca-path</span><br /><br /><span class="tdlppd">Path to server CA certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-ca-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-cert-path">--tls-cert-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-cert-path</span><br /><br /><span class="tdlppd">Path to x509 certificate.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-cert-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-disable-host-verification">--tls-disable-host-verification<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-disable-host-verification</span><br /><br /><span class="tdlppd">Disables TLS host name verification if already enabled.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-disable-host-verification">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-key-path">--tls-key-path<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-key-path</span><br /><br /><span class="tdlppd">Path to private certificate key.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-key-path">Learn more</a></span></span></a>

- <a class="tdlp" href="/cli/cmd-options#tls-server-name">--tls-server-name<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">temporal  tls-server-name</span><br /><br /><span class="tdlppd">Provides an override for the target TLS server name.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/cli/cmd-options#tls-server-name">Learn more</a></span></span></a>

