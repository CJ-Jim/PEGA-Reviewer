Designing an approval process

- [1. Work approval](#1-work-approval)
    - [Case approvals](#case-approvals)
    - [The Approve/Reject step](#the-approvereject-step)
    - [Routing](#routing)
    - [Routing notifications](#routing-notifications)
    - [Flow](#flow)

## 1. Work approval

### Case approvals

are decision points at which one or more users decide whether to approve or reject a case.

### The Approve/Reject step

To configure an Approve/Reject step, you define who is assigned to the approval and how the case proceeds if the case is approved or rejected. To achieve this, you configure the Approve/Reject step routing and flow.

### Routing

You can assign approvals to different routing options (e.g. specific user, work queue, and business logic)

### Routing notifications

**Email notification**

If the email approval option is enabled, when the case reaches the approval step, the application sends an email to the user or users specified by the step routing.

<img src="../resources/email-notification.png" width=600>

**Mobile notification**

If the mobile approval is enabled, the application pushes an approval notification to a mobile device.

<img src="../resources/mobile-notification.png" width=600>

### Flow

You configure the consequences of approval and rejection by defining the flow.

You can configure approvals to automatically:

- continue the case
- change to a specific stage
- change the case status

You can configure rejections to automatically:

- resolve a case
- continue the case
- change to a specific stage

<img src="../resources/approve-reject.png" width=300>
