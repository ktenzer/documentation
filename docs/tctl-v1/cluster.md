---
id: cluster
title: tctl v1.17 cluster command reference
sidebar_label: cluster
description: How to use the tctl v1.17 cluster command
toc_max_heading_level: 4
---

<!-- THIS FILE IS GENERATED. DO NOT EDIT THIS FILE DIRECTLY -->

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

:::success Temporal CLI is now available!

The new [Temporal CLI](/cli) is available for use.

tctl v1.17 can still be used with Temporal Server version 1.20 and is expected to be compatible with Temporal Server version 1.21.

tctl is expected to be fully deprecated by Temporal Server version 1.22

:::

The `tctl cluster` command enables <a class="tdlp" href="/clusters#">Temporal Cluster<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">What is a Temporal Cluster?</span><br /><br /><span class="tdlppd">A Temporal Cluster is the Temporal Server paired with persistence.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/clusters#">Learn more</a></span></span></a> operations.

- <a class="tdlp" href="#health">tctl cluster health<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">tctl cluster health</span><br /><br /><span class="tdlppd">How to check the health of the Frontend Service using tctl.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="#health">Learn more</a></span></span></a>
- <a class="tdlp" href="#get-search-attributes">tctl cluster get-search-attributes<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">tctl cluster get-search-attributes</span><br /><br /><span class="tdlppd">How to list all Search Attributes using tctl.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="#get-search-attributes">Learn more</a></span></span></a>

## get-search-attributes

The `tctl cluster get-search-attributes` command lists all <a class="tdlp" href="/visibility#search-attribute">Search Attributes<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">What is a Search Attribute?</span><br /><br /><span class="tdlppd">A Search Attribute is an indexed name used in List Filters to filter a list of Workflow Executions that have the Search Attribute in their metadata.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/visibility#search-attribute">Learn more</a></span></span></a> that can be used in the `--query` modifier of the <a class="tdlp" href="/tctl-v1/workflow#list">`tctl workflow list`<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">tctl workflow list</span><br /><br /><span class="tdlppd">How to list open or closed Workflow Executions using tctl.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/tctl-v1/workflow#list">Learn more</a></span></span></a> command and the `--search_attr_key` and `--search_attr_value` modifiers of the <a class="tdlp" href="/tctl-v1/workflow#run">`tctl workflow run`<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">tctl workflow run</span><br /><br /><span class="tdlppd">How to start a new Workflow Execution and get Workflow progress using tctl.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/tctl-v1/workflow#run">Learn more</a></span></span></a> and <a class="tdlp" href="/tctl-v1/workflow#start">`tctl workflow start`<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">tctl workflow start</span><br /><br /><span class="tdlppd">How to start a new Workflow Execution using tctl.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/tctl-v1/workflow#start">Learn more</a></span></span></a> commands.

**Example:**

```bash
tctl cluster get-search-attributes
```

The command has no modifiers.

Example output:

```text
+-----------------------+----------+
|         NAME          |   TYPE   |
+-----------------------+----------+
| BinaryChecksums       | Keyword  |
| CloseTime             | Int      |
| CustomBoolField       | Bool     |
| CustomDatetimeField   | Datetime |
| CustomDoubleField     | Double   |
| CustomIntField        | Int      |
| CustomKeywordField    | Keyword  |
| CustomNamespace       | Keyword  |
| CustomStringField     | String   |
| ExecutionStatus       | Int      |
| ExecutionTime         | Int      |
| Operator              | Keyword  |
| RunId                 | Keyword  |
| StartTime             | Int      |
| TaskQueue             | Keyword  |
| TemporalChangeVersion | Keyword  |
| WorkflowId            | Keyword  |
| WorkflowType          | Keyword  |
+-----------------------+----------+
```

The admin version of this command displays default and custom Search Attributes separately, and also shows the underlying Elasticsearch index schema and system Workflow status.

## health

The `tctl cluster health` command checks the health of the <a class="tdlp" href="/clusters#frontend-service">Frontend Service<span class="tdlpiw"><img src="/img/link-preview-icon.svg" alt="Link preview icon" /></span><span class="tdlpc"><span class="tdlppt">What is a Temporal Cluster?</span><br /><br /><span class="tdlppd">A Temporal Cluster is the Temporal Server paired with persistence.</span><span class="tdlplm"><br /><br /><a class="tdlplma" href="/clusters#frontend-service">Learn more</a></span></span></a>.

`tctl cluster health`

The command has no modifiers.

