**Anki-MedRec Platform - Internal APIs**
===================


This page describes the APIs that are required as part of **v1** for the  **MedRecNG**. 

----------


Physician
-------------

Physician is the person qualified to practise medicine, especially one who specialises in diagnosis and medical treatment.

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Full Name
- Medical speciality
- Prescriptions
- Agenda
- Availability for appointment

#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing physician(s)
> **/physicians** --`It returns the full list of physicians with all required attributes`
<br>
> **/physician/{id}**   -- `It returns the list of required attributes for this physician.`
<br>
> **/physician/{id}/agenda** -- `It returns the next 2 weeks agenda.`
<br>
> **/physician/{id}/availability**  -- `It returns the next 2 weeks availability.`
<br>
> **/physician/{id}/prescriptions**  -- `It returns the full list of prescriptions issued by this physician.`

- **PUT** -- Updates existing physician(s)
> **/physicians** -- `JSON payload with list of all physicians attributes attached, including Ids.`
<br>
> **/physician**   -- `JSON payload with all physician's attributes attached, including Id.`

- **POST** -- Creates new physician(s)
> **/physicians** -- `JSON payload with list of physicians attributes attached.`
<br>
> **/physician**   -- `JSON payload with physician's attributes attached.`

- **DELETE** -- Delete existing physician(s)
> **/physicians** -- `JSON payload with list of physicians Ids to be removed.`
<br>
> **/physician/{id}**   -- `Deletes Physician by Id.`

 
  
Patient
-------------

Patient is a person receiving or registered to receive medical treatment.

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Full Name
- Age
- Address
- Mobile
- Email
- Medical Conditions
- Medical Appointments
- Prescriptions
- Medical measures `-- See "Measures"`

#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing patient(s)
> **/patients** -- `It returns the full list of patients with all required attributes.`
<br>
> **/patient/{id}**   -- `It returns the list of required attributes for this patient.`
<br>
> **/patient/{id}/conditions**  -- `It returns the Patient's Medical Conditions.`
<br>
> **/patient/{id}/appointments** -- `It returns the patient's next 2 weeks appointments.`
<br>
> **/patient/{id}/prescriptions** -- `It returns the full list of prescriptions issued to this patient.`

- **PUT** -- Updates existing patient(s)
> **/patients** -- `JSON payload with list of patients attributes attached, including Ids.`
<br>
> **/patient**   -- `JSON payload with patient's attributes attached, including Id.`

- **POST** -- Creates new patient(s)
> **/patients** -- `JSON payload with list of patients attributes attached.`
<br>
> **/patient**   -- `JSON payload with patient's attributes attached.`

- **DELETE** -- Delete existing patient(s)
> **/patients** -- `JSON payload with list of patients Ids to be removed.`
<br>
> **/patient/{id}**   -- `Deletes a patient by Id.`


Appointments
-------------

Medical appointments between a Patient and a Physician in order to undergo a medical procedure.

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Name
- Physician Id
- Patient Id
- Day
- Time
- Notes

#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing appointment(s)
> **/appointments** -- `It returns the full list of existing appointments with all required attributes.`
<br>
> **/appointment/{id}**   -- `It returns the list of required attributes for this appointment.`

- **PUT** -- Updates existing appointment(s)
> **/appointments** -- `JSON payload with list of appointments attributes attached, including Ids.`
<br>
> **/appointment**   -- `JSON payload with appointment's attributes attached, including Id.`

- **POST** -- Creates new appointment(s)
> **/appointments** -- `JSON payload with list of appointments attributes attached.`
<br>
> **/appointment**   -- `JSON payload with appointment's attributes attached.`

- **DELETE** -- Delete existing appointment(s)
> **/appointments** -- `JSON payload with list of appointments Ids to be removed.`
<br>
> **/appointment/{id}**   -- `Deletes an appointment by Id.`


 
Prescriptions
-------------

Prescriptions are instructions written by a medical practitioner that authorises a patient to be issued with a medicine or treatment.

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Name
- Physician Id
- Patient Id
- Medical drugs  `See Drugs below`
- Notes


#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing prescription(s)
> **/prescriptions** -- `It returns the full list of issued prescriptions with all required attributes.`
<br>
> **/prescription/{id}**   -- `It returns the list of required attributes for this prescription.`

- **PUT** -- Updates existing prescription(s)
> **/prescriptions** -- `JSON payload with list of prescriptions attributes attached, including Ids.`
<br>
> **/prescription**   -- `JSON payload with prescription's attributes attached, including Id.`

- **POST** -- Creates new prescription(s)
> **/prescriptions** -- `JSON payload with list of prescriptions attributes attached.`
<br>
> **/prescription**   -- `JSON payload with prescription's attributes attached.`

- **DELETE** -- Delete existing prescription(s)
> **/prescriptions** -- `JSON payload with list of prescriptions Ids to be removed.`
<br>
> **/prescription/{id}**   -- `Deletes a prescription by Id.`

  
Measures
-------------

Patients Medical Measures are a series of constant recordings on a patient's record that help understand pre-existing conditions, diagnosis and potential treatments. Examples of Patient's Medical measures are: weight, temperature, blood pressure, stress level, heart beat, etc.

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Patient Id
- Name
- Type
- Recording device 
- Date of measure
- Notes


#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing patient's medical measure(s)
> **/measures** -- `It returns the full list of measures with all required attributes.`
<br>
> **/measure/patient/{id}**   -- `It returns the list of measures conducted on patient id`

- **POST** -- Creates new patient's medical measure(s)
> **/measures** -- `JSON payload with list of full patients list medical measures attached. This API is merely used for maintenance/data recovery purposes.`
<br>
> **/measure/patient/{id}**   -- `JSON payload with a new patient medical measure  attached.`

- **DELETE** -- Delete existing patient's medical measure(s)
> **/measures** -- `JSON payload with list of measures Ids to be removed. - This API is merely used for maintenance purposes.`
<br>
> **/measure/patient/{id}**   -- `Deletes ALL existing patient's medical measures. - This API is merely used for maintenance purposes.`

   

Drugs
-------------

A pharmaceutical drug (also referred to as medicine, medication, or simply as drug) is a drug used to diagnose, cure, treat, or prevent disease.

    Note: This is just an inventory of Drugs. In order to prescribe drugs, see "Prescriptions"

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Name
- Formula
- Side effects

#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing drug(s)
> **/drugs** -- `It returns the full list of existing drugs in the inventory with all required attributes.`
<br>
> **/drug/{id}**   -- `It returns the list of required attributes for this drup.`

- **PUT** -- Updates existing drug(s)
> **/drugs** -- `JSON payload with list of drugs attributes attached, including Ids.`
<br>
> **/drug**   -- `JSON payload with drug's attributes attached, including Id.`

- **POST** -- Creates new drug(s)
> **/drugs** -- `JSON payload with list of drugs attributes attached.`
<br>
> **/drug**   -- `JSON payload with drug's attributes attached.`

- **DELETE** -- `Delete existing drug(s)`
> **/drugs** -- `JSON payload with list of drugs Ids to be removed.`
<br>
> **/drug/{id}**   -- `Deletes an drug by Id.`


Diseases
-------------

A disease is a disorder of structure or function in a human, animal, or plant, especially one that produces specific symptoms or that affects a specific location and is not simply a direct result of physical injury.

    Note: This is just an catalogue of Diseases. In order to prescribe treatments, see "Prescriptions"

#### <i class="icon-file"></i> Required attributes:

The list below shows only those attributes that are required for v1. It is expected that other attributes are being inherited by MedRec app.
- Id
- Name
- Symptoms
- Treatment

#### <i class="icon-file"></i> Required APIs:

    Note: At this point, the format for the JSON request & response is **open for interpretation**.

- **GET** -- Get existing disease(s)
> **/diseases** -- `It returns the full list of existing diseases in the catalogue with all required attributes.`
<br>
> **/disease/{id}**   -- `It returns the list of required attributes for this disease.`

- **PUT** -- Updates existing disease(s)
> **/diseases** -- `JSON payload with list of diseases attributes attached, including Ids.`
<br>
> **/disease**   -- `JSON payload with disease's attributes attached, including Id.`

- **POST** -- Creates new disease(s)
> **/diseases** -- `JSON payload with list of diseases attributes attached.`
<br>
> **/disease**   -- `JSON payload with disease's attributes attached.`

- **DELETE** -- `Delete existing disease(s)`
> **/diseases** -- `JSON payload with list of diseases Ids to be removed.`
<br>
> **/disease/{id}**   -- `Deletes a disease by Id.`



----------

<a href="index" rel="Go back">![link text](./img/back.png "Go Back")</a>

