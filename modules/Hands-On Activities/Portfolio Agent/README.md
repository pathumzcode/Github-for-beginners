# 🤖 Build a Portfolio Generation Agent

In this hands-on activity, you will create and use a custom **Portfolio Generation Agent** with **GitHub Copilot CLI**.

The agent will analyze a user's CV or profile information and use the verified information to create a professional, responsive personal portfolio website.

By completing this activity, you will learn how to:

* Create a custom GitHub Copilot CLI Agent
* Run a custom Agent using GitHub Copilot CLI
* Provide a CV as input
* Analyze CV information
* Generate a professional portfolio website
* Review an AI-generated portfolio
* Work safely with AI-assisted development

---

# 📚 Content

| Step                                                        | Activity                              | Description                                                                          |
| ----------------------------------------------------------- | ------------------------------------- | ------------------------------------------------------------------------------------ |
| [Step 01](#step-01---start-copilot-cli)                     | Start GitHub Copilot CLI              | Launch GitHub Copilot CLI.                                                           |
| [Step 02](#step-02---check-your-custom-agents)              | Check Your Custom Agents              | Check the available custom agents.                                                   |
| [Step 03](#step-03---create-your-agent-through-the-cli)     | Create the Portfolio Generation Agent | Create the custom Agent using the Copilot CLI.                                       |
| [Step 04](#step-04---check-the-custom-agent)                | Check the Custom Agent                | Confirm that the Portfolio Generation Agent is available.                            |
| [Step 05](#step-05---startrestart-github-copilot-cli)       | Start/Restart GitHub Copilot CLI      | Start or restart Copilot CLI after creating the Agent.                               |
| [Step 06](#step-06---select-the-portfolio-generation-agent) | Select the Portfolio Generation Agent | Select the custom Agent from the `/agent` menu.                                      |
| [Step 07](#step-07---provide-and-analyze-your-cv)           | Provide and Analyze Your CV           | Provide your CV and verify the information identified by the Agent.                  |
| [Step 08](#step-08---generate-the-portfolio)                | Generate the Portfolio                | Generate the portfolio using the verified CV information.                            |
| [Step 09](#step-09---review-the-portfolio)                  | Review the Portfolio                  | Ask the Agent to review the generated portfolio and identify important improvements. |

---

# ⚠️ Important

Complete this activity using **GitHub Copilot CLI**.

You should understand and review the commands, plans, file changes, and code proposed by the AI before approving them.

**Do not blindly approve AI-generated changes.**

---

# 🛠️ Step-by-Step Activities

## Step 01 - Start Copilot CLI

Run GitHub Copilot CLI using the command below:

```powershell
copilot
```

The `copilot` command launches the interactive GitHub Copilot CLI.

---

## Step 02 - Check Your Custom Agents

Once Copilot opens, type:

```text
/agent
```

This opens the Agent selector and shows the available custom agents.

If you have not created any custom agents yet, the list may be empty.


![Empty Agent List](/images/empty_agent_list.png)

---

## Step 03 - Create Your Agent Through the CLI

Press:

```text
n
```

This starts the process of creating a new custom Agent.

Copilot will ask you for the Agent details.

### Agent Scope

Choose the appropriate scope:

> Choose **Project** to make the Agent available within this project, or choose **User** if you prefer to use it across your personal projects.

For this workshop, **Project** is recommended because the Agent is being created for this project.

### Agent Name

Use:

```text
portfolio-generation
```

Simply press **Enter** to continue.

### Description

The complete Agent configuration and instructions are available here:

[View Portfolio Generation Agent Description](./resources/Portfolio%20Generation%20Agent/portfolio-generation.agent.md)

### Tool Selection

Select the tools required by the Agent to inspect, search, modify, and test the project.

For the Portfolio Generation Agent, you can keep the default tool access or restrict the available tools according to the requirements of your project.

> 🎉 **Successfully created your custom agent!**

---

## Step 04 - Check the Custom Agent

After creating the Agent, verify that it is available in GitHub Copilot CLI.

### 1. Open GitHub Copilot CLI

```powershell
copilot
```

### 2. Open the Agent selector

```text
/agent
```

### 3. Find and select

```text
portfolio-generation
```

### 4. Confirm the Agent

Confirm that the **Portfolio Generation** Agent is available and ready to use.

> **Tip:** If the Agent does not appear, restart GitHub Copilot CLI and run `/agent` again.

---

## Step 05 - Start/Restart GitHub Copilot CLI

If you created the Agent during the previous session, restart GitHub Copilot CLI so the newly created Agent is loaded.

Run:

```powershell
copilot
```

Then open the Agent selector:

```text
/agent
```

---

## Step 06 - Select the Portfolio Generation Agent

From the `/agent` menu, select:

```text
portfolio-generation
```

Confirm that the **Portfolio Generation** Agent is now selected and ready to use.

---

## Step 07 - Provide and Analyze Your CV

Provide your CV or profile information to the Portfolio Generation Agent.

Use a prompt similar to the following:

```text
Analyze my CV and identify the verified information that can be used to create my personal portfolio.

Do not modify any project files yet.

First, summarize:
- Personal information
- About/profile information
- Education
- Skills
- Projects
- Experience
- Certifications
- Achievements
- Community activities
- Contact information

Do not invent or assume any information that is not provided in my CV.
```

Review the information identified by the Agent.

Make sure the extracted information is accurate before continuing.

---

## Step 08 - Generate the Portfolio

After verifying the CV information, ask the Agent to create the portfolio.

Use a prompt similar to the following:

```text
Create my personal portfolio using the verified information from my CV.

Use the supplied visual reference as design inspiration only.

Create a professional, responsive, and accessible portfolio while preserving the existing project structure and technology stack.

Do not invent any information.

Before making file changes, provide an implementation plan for review.
```

Review the implementation plan provided by the Agent.

After reviewing the plan, approve the changes so the Agent can implement the portfolio.

---

## Step 09 - Review the Portfolio

After the portfolio has been generated, ask the Agent to review the implementation.

Use a prompt similar to the following:

```text
Review the generated portfolio.

Check:
- Content accuracy
- Responsive design
- Visual hierarchy
- Layout and spacing
- Accessibility
- Navigation
- Mobile responsiveness
- Typography
- Image usage
- Overall consistency

Identify the most important improvements that could be made.

Do not make changes yet.
```

Review the feedback provided by the Agent.

At this stage, you can discuss the suggested improvements with the Agent and decide which changes you want to make.

---

# 🎉 Activity Completed

Congratulations! You have successfully created and used a custom **Portfolio Generation Agent** with **GitHub Copilot CLI**.

You have learned how to:

* Create a custom Copilot CLI Agent
* Configure an Agent for a specific task
* Select and use a custom Agent
* Analyze verified CV information
* Generate a professional portfolio
* Review an AI-generated website
* Work safely with AI-assisted development
