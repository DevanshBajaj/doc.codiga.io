---
id: integration-gitlab
title: Gitlab Integration
description: Check your code quality with Codiga for all GitLab repositories. Work for for 12+ languages. Free 14 days trial.
keywords:
  [
    gitlab,
    continous deployment,
    codiga,
    static analysis,
    static code analysis,
    continuous integration,
    ci/cd pipeline,
    code verification,
    security analysis,
    CWE,
    CVE,
  ]
---

## Gitlab Accounts

You can log into Codiga using your Gitlab credentials.
Your account is then automatically linked with Gitlab and you
can easily add Gitlab repositories in your Codiga projects.

## Supported features

- Login
- Import Gitlab repositories
- Code Reviews on Merge Requests
- Automated Code Fix (silver and gold accounts)

## Webhook

In order to have code reviews and analyses on push, you need to
make sure webhooks are activated.

Codiga installs a webhook when you import a Gitlab project.
However, you may have deleted it yourself and/or removed it in the past.

Make sure the webhook is activated. You can activate the webhook in your
project preferences on Codiga.

![Preferences for Gitlab webhook](/img/gitlab-webhook-preferences.png)

Once you create the webhook from Codiga, you should see
a webhook appearing in your Gitlab preferences too, as shown below.

![Webhook on Gitlab](/img/gitlab-webhook-preferences-gitlab.png)

If the webhook is not created, it is because the user attempting to create
the webhook does not have enough permission to create a webhook. In that
case, you will need to upgrade this user permission or use another
account to manage this project on Codiga.

## Code Reviews

Codiga will do automated code reviews on merge requests. For
each new commit, the platform will annotate the code with violations
it found, as shown below.

![Gitlab Code Review](/img/gitlab-code-review-example.png)

The Code Review will be done with the account that created the repository.
You may want to use a service account (e.g. an account that does not
belong to a developer) to do the code review to distinguish comments
from the automated code review from the one from developers.

In that case, creates the project with the service account. You can
also contact us to change the owner of the project and associate it
with the service account. To do so, make sure the service account is
registered on Codiga and send us the project and the name of
the service account, we can change the owner of the project.
