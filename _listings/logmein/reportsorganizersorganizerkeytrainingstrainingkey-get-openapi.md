---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToTraining Get Sessions by Training
  description: Get sessions by training.
  version: 1.0.0
host: api.getgo.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/trainings:
    get:
      summary: Get Trainings
      description: Get trainings.
      operationId: OrganizersTrainingsByOrganizerKeyGet
      x-api-path-slug: organizersorganizerkeytrainings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      responses:
        200:
          description: OK
      tags:
      - Trainings
    post:
      summary: Create Training
      description: Create training.
      operationId: OrganizersTrainingsByOrganizerKeyPost
      x-api-path-slug: organizersorganizerkeytrainings-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      responses:
        200:
          description: OK
      tags:
      - Training
  /trainings/{trainingKey}/start:
    get:
      summary: Start Training
      description: Start training.
      operationId: TrainingsStartByTrainingKeyGet
      x-api-path-slug: trainingstrainingkeystart-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Start
      - Training
  /organizers/{organizerKey}/trainings/{trainingKey}/organizers:
    put:
      summary: Update Training Organizers
      description: Update training organizers.
      operationId: OrganizersTrainingsOrganizersByOrganizerKeyAndTrainingKeyPut2
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Organizers
  /reports/organizers/{organizerKey}/trainings/{trainingKey}:
    get:
      summary: Get Sessions by Training
      description: Get sessions by training.
      operationId: ReportsOrganizersTrainingsByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Sessions
      - By
      - Training
  /organizers/{organizerKey}/trainings/{trainingKey}/registrationSettings:
    put:
      summary: Update Training Registration Settings
      description: Update training registration settings.
      operationId: OrganizersTrainingsRegistrationSettingsByOrganizerKeyAndTrainingKeyPut
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Registration
      - Settings
  /organizers/{organizerKey}/trainings/{trainingKey}:
    get:
      summary: Get Training
      description: Get training.
      operationId: OrganizersTrainingsByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
    delete:
      summary: Delete Training
      description: Delete training.
      operationId: OrganizersTrainingsByOrganizerKeyAndTrainingKeyDelete
      x-api-path-slug: organizersorganizerkeytrainingstrainingkey-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
  '/organizers/{organizerKey}/trainings/{trainingKey}/registrants ':
    get:
      summary: Get Training Registrants
      description: Get training registrants.
      operationId: OrganizersTrainingsRegistrantsByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Registrants
  /organizers/{organizerKey}/trainings/{trainingKey}/times:
    put:
      summary: Update Training Times
      description: Update training times.
      operationId: OrganizersTrainingsTimesByOrganizerKeyAndTrainingKeyPut
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeytimes-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Times
  /organizers/{organizerKey}/trainings/{trainingKey}/nameDescription:
    put:
      summary: Update Training Name and Description
      description: Update training name and description.
      operationId: OrganizersTrainingsNameDescriptionByOrganizerKeyAndTrainingKeyPut
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeynamedescription-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Name
      - Description
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