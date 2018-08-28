---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Trainings
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Training - Get Trainings
  x-api-slug: organizersorganizerkeytrainings-get
  description: This call retrieves information on all scheduled trainings for a given
    organizer. The trainings are returned in the order in which they were created.
    Completed trainings are not included; ongoing trainings with past sessions are
    included along with the past sessions. If the organizer does not have any scheduled
    trainings, the response will be empty.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainings-get-openapi.md
- name: Go To Training - Create Training
  x-api-slug: organizersorganizerkeytrainings-post
  description: Schedules a training of one or more sessions. The call requires a training's
    name, at least one start and end time, and optionally may include additional sessions,
    a description, additional organizers (presenters), and registration settings.
    You can only add organizers to a training if you have a multi-user account. Once
    a training has been created with this method, you can accept registrations to
    the training. Registration is for the entire training - all sessions. (The GoToTraining
    admin site enables you to create trainings that allow participants to register
    for individual sessions as well as automatically create weekly or monthly events.)
    Registration settings controls whether you allow web registration for this training,
    and whether a confirmation email is sent to the registrant following registration.
    Disabling the confirmation email is an API-only setting. If the user registers
    through the GoToTraining website, a confirmation email is sent. If the user is
    manually approved by the training administrator through the GoToTraining web site,
    the confirmation email is sent. It is recommended that you disable web registration
    if you disable confirmation emails. The response contains a trainingKey for the
    scheduled training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainings-post-openapi.md
- name: Go To Training - Delete Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-delete
  description: 'Deletes a scheduled or completed training. For scheduled trainings,
    it deletes all scheduled sessions of the training. For completed trainings, the
    sessions remain in the database. No email is sent to organizers or registrants,
    but when participants attempt to start or join the training, they are directed
    to a page that states: Training Not Found: The training you are trying to join
    is no longer available.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-delete-openapi.md
- name: Go To Training - Get Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-get
  description: Uses the organizer key and training key to retrieve information on
    a scheduled training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Management URL for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeymanageurl-get
  description: A request for a direct URL to the admin portal for a specific training.
    The request identifies the organizer and the training; the response provides a
    link the organizer can use to manage or launch the training in the admin portal.
    The training organizer will be required to log in. You can schedule and manage
    the training (e.g., add tests, polls and training materials) from the URL provided
    in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeymanageurl-get-openapi.md
- name: Go To Training - Update Training Name and Description
  x-api-slug: organizersorganizerkeytrainingstrainingkeynamedescription-put
  description: Request to update a scheduled training name and description.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeynamedescription-put-openapi.md
- name: Go To Training - Get Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-get
  description: Retrieves organizer details for a specific training. This is only applicable
    to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-get-openapi.md
- name: Go To Training - Update Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
  description: Replaces the co-organizers for a specific training. The scheduling
    organizer cannot be unassigned. Organizers will be notified via email if the notifyOrganizers
    parameter is set to true. Replaced organizers are not notified. This method is
    only applicable to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-put-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start after the organizer logs in with its credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
- name: Go To Training - Update Training Times
  x-api-slug: organizersorganizerkeytrainingstrainingkeytimes-put
  description: A request to update a scheduled training's start and end times. If
    the request contains 'notifyTrainers = true' and 'notifyRegistrants = true', both
    organizers and registrants are notified. The response provides the number of notified
    trainers and registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeytimes-put-openapi.md
- name: Go To Training - Get Sessions By Training
  x-api-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
  description: This call returns session details for a given training. A session is
    a completed training event. Each training may contain one or more sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/reportsorganizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Online Recordings for Training
  x-api-slug: trainingstrainingkeyrecordings-get
  description: This call retrieves information on all online recordings for a given
    training. If there are none, it returns an empty list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-openapi.md
- name: Go To Training - Get Download for Online Recordings
  x-api-slug: trainingstrainingkeyrecordingsrecordingid-get
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-openapi.md
- name: Go To Training - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start. A login of the organizer is not required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeystart-get-openapi.md
- name: Go To Training - Delete Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-delete
  description: 'Deletes a scheduled or completed training. For scheduled trainings,
    it deletes all scheduled sessions of the training. For completed trainings, the
    sessions remain in the database. No email is sent to organizers or registrants,
    but when participants attempt to start or join the training, they are directed
    to a page that states: Training Not Found: The training you are trying to join
    is no longer available.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-delete-openapi.md
- name: Go To Training - Get Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-get
  description: Uses the organizer key and training key to retrieve information on
    a scheduled training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Management URL for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeymanageurl-get
  description: A request for a direct URL to the admin portal for a specific training.
    The request identifies the organizer and the training; the response provides a
    link the organizer can use to manage or launch the training in the admin portal.
    The training organizer will be required to log in. You can schedule and manage
    the training (e.g., add tests, polls and training materials) from the URL provided
    in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeymanageurl-get-openapi.md
- name: Go To Training - Update Training Name and Description
  x-api-slug: organizersorganizerkeytrainingstrainingkeynamedescription-put
  description: Request to update a scheduled training name and description.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeynamedescription-put-openapi.md
- name: Go To Training - Get Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-get
  description: Retrieves organizer details for a specific training. This is only applicable
    to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-get-openapi.md
- name: Go To Training - Update Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
  description: Replaces the co-organizers for a specific training. The scheduling
    organizer cannot be unassigned. Organizers will be notified via email if the notifyOrganizers
    parameter is set to true. Replaced organizers are not notified. This method is
    only applicable to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-put-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start after the organizer logs in with its credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
- name: Go To Training - Update Training Times
  x-api-slug: organizersorganizerkeytrainingstrainingkeytimes-put
  description: A request to update a scheduled training's start and end times. If
    the request contains 'notifyTrainers = true' and 'notifyRegistrants = true', both
    organizers and registrants are notified. The response provides the number of notified
    trainers and registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeytimes-put-openapi.md
- name: Go To Training - Get Sessions By Training
  x-api-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
  description: This call returns session details for a given training. A session is
    a completed training event. Each training may contain one or more sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/reportsorganizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Online Recordings for Training
  x-api-slug: trainingstrainingkeyrecordings-get
  description: This call retrieves information on all online recordings for a given
    training. If there are none, it returns an empty list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-openapi.md
- name: Go To Training - Get Download for Online Recordings
  x-api-slug: trainingstrainingkeyrecordingsrecordingid-get
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-openapi.md
- name: Go To Training - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start. A login of the organizer is not required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeystart-get-openapi.md
- name: Go To Training - Delete Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-delete
  description: 'Deletes a scheduled or completed training. For scheduled trainings,
    it deletes all scheduled sessions of the training. For completed trainings, the
    sessions remain in the database. No email is sent to organizers or registrants,
    but when participants attempt to start or join the training, they are directed
    to a page that states: Training Not Found: The training you are trying to join
    is no longer available.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-delete-openapi.md
- name: Go To Training - Get Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-get
  description: Uses the organizer key and training key to retrieve information on
    a scheduled training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Management URL for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeymanageurl-get
  description: A request for a direct URL to the admin portal for a specific training.
    The request identifies the organizer and the training; the response provides a
    link the organizer can use to manage or launch the training in the admin portal.
    The training organizer will be required to log in. You can schedule and manage
    the training (e.g., add tests, polls and training materials) from the URL provided
    in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeymanageurl-get-openapi.md
- name: Go To Training - Update Training Name and Description
  x-api-slug: organizersorganizerkeytrainingstrainingkeynamedescription-put
  description: Request to update a scheduled training name and description.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeynamedescription-put-openapi.md
- name: Go To Training - Get Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-get
  description: Retrieves organizer details for a specific training. This is only applicable
    to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-get-openapi.md
- name: Go To Training - Update Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
  description: Replaces the co-organizers for a specific training. The scheduling
    organizer cannot be unassigned. Organizers will be notified via email if the notifyOrganizers
    parameter is set to true. Replaced organizers are not notified. This method is
    only applicable to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-put-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start after the organizer logs in with its credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
- name: Go To Training - Update Training Times
  x-api-slug: organizersorganizerkeytrainingstrainingkeytimes-put
  description: A request to update a scheduled training's start and end times. If
    the request contains 'notifyTrainers = true' and 'notifyRegistrants = true', both
    organizers and registrants are notified. The response provides the number of notified
    trainers and registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeytimes-put-openapi.md
- name: Go To Training - Get Sessions By Training
  x-api-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
  description: This call returns session details for a given training. A session is
    a completed training event. Each training may contain one or more sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/reportsorganizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Get Online Recordings for Training
  x-api-slug: trainingstrainingkeyrecordings-get
  description: This call retrieves information on all online recordings for a given
    training. If there are none, it returns an empty list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-openapi.md
- name: Go To Training - Get Download for Online Recordings
  x-api-slug: trainingstrainingkeyrecordingsrecordingid-get
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-openapi.md
- name: Go To Training - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start. A login of the organizer is not required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeystart-get-openapi.md
- name: Go To Training - Start Training
  x-api-slug: trainingstrainingkeystart-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start. A login of the organizer is not required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeystart-get-openapi.md
- name: Go To Training - Get Download for Online Recordings
  x-api-slug: trainingstrainingkeyrecordingsrecordingid-get
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-openapi.md
- name: Go To Training - Get Online Recordings for Training
  x-api-slug: trainingstrainingkeyrecordings-get
  description: This call retrieves information on all online recordings for a given
    training. If there are none, it returns an empty list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-openapi.md
- name: Go To Training - Get Sessions By Training
  x-api-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
  description: This call returns session details for a given training. A session is
    a completed training event. Each training may contain one or more sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/reportsorganizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Update Training Times
  x-api-slug: organizersorganizerkeytrainingstrainingkeytimes-put
  description: A request to update a scheduled training's start and end times. If
    the request contains 'notifyTrainers = true' and 'notifyRegistrants = true', both
    organizers and registrants are notified. The response provides the number of notified
    trainers and registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeytimes-put-openapi.md
- name: Go To Training - Get Start Url
  x-api-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
  description: Returns a URL that can be used to start a training. When this URL is
    opened in a web browser, the GoToTraining client will be downloaded and launched
    and the training will start after the organizer logs in with its credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeystarturl-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Update Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
  description: Replaces the co-organizers for a specific training. The scheduling
    organizer cannot be unassigned. Organizers will be notified via email if the notifyOrganizers
    parameter is set to true. Replaced organizers are not notified. This method is
    only applicable to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-put-openapi.md
- name: Go To Training - Get Training Organizers
  x-api-slug: organizersorganizerkeytrainingstrainingkeyorganizers-get
  description: Retrieves organizer details for a specific training. This is only applicable
    to multi-user accounts with sharing enabled (co-organizers).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyorganizers-get-openapi.md
- name: Go To Training - Update Training Name and Description
  x-api-slug: organizersorganizerkeytrainingstrainingkeynamedescription-put
  description: Request to update a scheduled training name and description.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeynamedescription-put-openapi.md
- name: Go To Training - Get Management URL for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeymanageurl-get
  description: A request for a direct URL to the admin portal for a specific training.
    The request identifies the organizer and the training; the response provides a
    link the organizer can use to manage or launch the training in the admin portal.
    The training organizer will be required to log in. You can schedule and manage
    the training (e.g., add tests, polls and training materials) from the URL provided
    in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeymanageurl-get-openapi.md
- name: Go To Training - Get Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-get
  description: Uses the organizer key and training key to retrieve information on
    a scheduled training.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-get-openapi.md
- name: Go To Training - Delete Training
  x-api-slug: organizersorganizerkeytrainingstrainingkey-delete
  description: 'Deletes a scheduled or completed training. For scheduled trainings,
    it deletes all scheduled sessions of the training. For completed trainings, the
    sessions remain in the database. No email is sent to organizers or registrants,
    but when participants attempt to start or join the training, they are directed
    to a page that states: Training Not Found: The training you are trying to join
    is no longer available.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/trainings/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkey-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.url.shortener.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gotomeeting.stack.network
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---