# SQS Dead-Letter Queues

## Understanding the Challenge

Amazon SQS supports dead-letter queues, which other queues (source queues) can target for
messages that can't be processed (consumed) successfully.

<p align="center">
  <img src="images/image1.png" alt="Image 1" width="45%" style="margin-right: 20px;" />
  <img src="images/image2.png" alt="Image 2" width="45%" />
</p>

## Moving to Dead-Letter Queue

Move the message that cannot be processed to dead letter queue.

![My Image](images/image3.png)

Move the the message that cannot be processed to dead letter queue.

![My Image](images/image4.png)

## Overview of Dead Letter Queue

Amazon SQS supports dead-letter queues, which other queues (source queues) can target for
messages that can't be processed (consumed) successfully
Dead-letter queues are useful for debugging your application or messaging system because
they let you isolate problematic messages to determine why their processing doesn't succeed.
The messages are sent to the dead letter queue after exceeding maximum receives.

## Important Pointers to Remember

When a message moves to a dead-letter queue, the timestamp remains unchanged.
Let’s understand this with an example:
- Message has been in the source queue for 1 day and moved to dead-letter queue.
- Message Retention Period in Dead Letter Queue is 4 days.
- Message will be deleted from the Dead Letter queue after 3 days.
Best practice is to have higher retention period for dead-letter queues then the source
queue.
