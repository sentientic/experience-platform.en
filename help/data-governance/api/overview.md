---
keywords: Experience Platform;home;popular topics
solution: Experience Platform
title: Policy Service API developer guide
topic: developer guide
---

# [!DNL Policy Service] API developer guide

Adobe Experience Platform [!DNL Data Governance] allows you to manage customer data and ensure compliance with regulations, restrictions, and policies applicable to data use. It plays a key role within [!DNL Experience Platform] at various levels, including cataloging, data lineage, data usage labeling, data usage policies, and controlling usage of data for marketing actions.

The [!DNL Policy Service] API provides several endpoints that allow you to programmatically manage data usage labels and policies, as well as evaluate marketing actions for policy violations. These endpoints are outlined below. Please visit the individual endpoint guides for details and refer to the [getting started guide](./getting-started.md) for important information on required headers, reading sample API calls, and more.

To view all available endpoints and CRUD operations, visit the [Policy Service API swagger](https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/dule-policy-service.yaml).

## Labels

Data usage labels allow you to categorize datasets and fields according to usage policies that apply to that data. Labels can be applied at any time, providing flexibility in how you choose to govern data. Best practices encourage labeling data as soon as it is ingested into [!DNL Experience Platform], or as soon as data becomes available for use in [!DNL Platform]. You can created, view, edit, and delete labels using the `/labels` endpoint. To learn how to use this endpoint, visit the [labels endpoint guide](./labels.md).

## Marketing actions

Marketing actions (also called marketing use cases), in the context of the [!DNL Data Governance] framework, are actions that an [!DNL Experience Platform] data consumer can take, for which your organization wants to restrict data usage. For detailed information on working with marketing actions, see the [marketing actions endpoint guide](./marketing-actions.md).

## Policies

Data usage policies are rules that describe the kinds of marketing actions that you are allowed to, or restricted from, performing on data within [!DNL Experience Platform]. A policy is defined by the following:

1. A specific marketing action
1. The data usage label(s) that action is restricted from being performed against

To learn how to manage policies in the API, see the [policies endpoint guide](./policies.md)

## Evaluation

Once data usage labels have been applied to [!DNL Platform] datasets, and data usage policies have been defined for marketing actions against those labels, Data Governance capabilities allow you to enforce those policies and prevent data operations that constitute policy violations.

The [!DNL Policy Service] API provides endpoints that allow you to test marketing actions against datasets or arbitrary combinations of data usage labels in order to check if any policy violations occur. Based on the API response, you can then set up protocols within your experience application to appropriately enforce data usage policy compliance. See the [evaluation endpoints guide](./evaluation.md) for more information.

## Next steps

To begin making calls using the [!DNL Policy Service] API, read the [getting started guide](./getting-started.md) then select one of the endpoint guides to learn how to use specific endpoints. To work with labels and policies using the [!DNL Experience Platform] UI, please refer to the [labels user guide](../labels/user-guide.md) and [policies user guide](../policies/user-guide.md), respectively.