---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Update Queue Members In Front
  description: Posting a URL and Method to a Queue instance will dequeue a member
    from anqueue and have the members call begin executing the TwiML document at that
    URLnWhen dequeuing the Front of the queue, the next call in the queue will be
    redirected.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Queues/{QueueSid}/Members/Front:
    get:
      summary: Get Queue Members In Front
      description: Get a front member.
      operationId: get-a-front-member
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembersfront-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
    post:
      summary: Update Queue Members In Front
      description: Posting a URL and Method to a Queue instance will dequeue a member
        from anqueue and have the members call begin executing the TwiML document
        at that URLnWhen dequeuing the Front of the queue, the next call in the queue
        will be redirected.n
      operationId: posting-a-url-and-method-to-a-queue-instance-will-dequeue-a-member-from-aqueue-and-have-the-members-
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembersfront-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---