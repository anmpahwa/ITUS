# Indian Time Use Survey - 2024

This sub-folder contains processed data from the 2024 Indian Time Use Survey conducted by the National Sample Survey Office (NSSO) under Ministry of Statistics and Programme Implementation (MoSPI), Government of India.

## Household Data

File: household.csv
Tag: Descriptive identification of sample households.
Columns:
- survey_year: 2024
- fsu_serial_no: first stage unit serial number
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- nss_region: National Service Scheme region code (refer to List of NSS Regions)
- district: district code (refer to List of States and Districts)
- stratum: stratum code
- sub_stratum: sub stratum code
- sub_round: survey round
    - 1: jan - mar
    - 2: apr - jun
    - 3: jul - sep
    - 4: oct - dec
- fod_sub_region: Field Operational Division of National Sample Survey Office (refer to List of FOD Sub-Regions)
- nsc: number of first stage units surveyed within a stratum x substratum for each state x sector
- household_id: household identity code
- informant_id: individual identity code (individual_id) of the informant
    - x: household member
    - 990: household non-member
- response_code: informant response
    - 1: co-operative and capable
    - 2: co-operative but not capable
    - 3: busy
    - 4: reluctant
    - 9: others
- survey_code: status of household survey
    - 1: original
    - 2: substitute
    - 3: casualty
- substitution_code: reason for substitution of original household
    - 1: informant busy
    - 2: members away from home
    - 3: informant non-cooperative
    - 9: others
- time_to_canvass: total time taken to canvass the survey by the team of investigators
- household_size: number of members of the household
- religion: household religion
    - 1: hinduism
    - 2: islam
    - 3: christianity
    - 4: sikhism
    - 5: jainism
    - 6: buddhism
    - 7: zoroastrianism
    - 9: others
- social_group
    - 1: scheduled tribe
    - 2: scheduled caste
    - 3: other backward class
    - 4: others
- land_possessed
    - 99: 0.00 hectare
    - 1: < 0.01 hectare
    - 2: [0.01, 0.05) hectare
    - 3: [0.05, 0.5) hectare
    - 4: [0.5, 1.0) hectare
    - 5: [1.0, 2.5) hectare
    - 6: [2.5, 5.0) hectare
    - 7: [5.0, 7.5) hectare
    - 8: [7.5, 10.0) hectare
    - 10: [10.0, 15.0) hectare
    - 11: [15.0, 20.0) hectare
    - 12: >= 20 hectare
- expenditure_pcs: monthly consumer expenditure for household purposes out of purchase
- expenditure_hgs: monthly consumer expenditure from home grown stock (imputed value)
- expenditure_osc: monthly consumer expenditure from other sources such as wages in kind, free collection, gifts, etc. (imputed value)
- expenditure_cfs: monthly consumer expenditure on clothing, footwear etc. during last 365 days
- expenditure_hds: monthly consumer expenditure on household durables
- total_expenditure: total monthly expenditure
- energy_cooking: primary source of energy for cooking during last 30 days
    - 1: firewood and chips
    - 2: LPG
    - 3: other natural gas
    - 4: dung cake
    - 5: kerosene
    - 6: coke orcoal
    - 7: gobar gas
    - 8: other biogas
    - 10: charcoal
    - 11: electricity
    - 12: no cooking arrangement
    - 19: others
- energy_lighting: primary source of energy for lighting during last 30 days
    - 1: electricity
    - 2: kerosene
    - 3: other oil
    - 4: gas
    - 5: candle
    - 6: no lighting arrangement
    - 9: others
- clothes_wash: primary type of washing of clothes during last 30 days
    - 1: mechanical by household members
    - 2: manual by household members
    - 3: outsourced
- floor_sweep: primary type of sweeping of floor during last 30 days
    - 1: mechanical by household members
    - 2: manual by household members
    - 3: outsourced
- dwelling_unit: type of dwelling unit
    - 1: owned
    - 2: hired
    - 3: no dwelling unit
    - 9: others
- dwelling_structure: type of the structure of the dwelling unit
    - 1: kutcha
    - 2: semi pucca
    - 3: pucca
- special_care: is there any member in the household aged 5 years and above who needs special care?
    - 1: yes
    - 2: no
- care giver: is there any care giver available among the household members for caring the person(s)?
    - 1: yes
    - 2: no
- weight: survey weight assigned to the household

#### Note
1. All missing data is represented by 99999, 
2. Definition data mismatch for stratum and sub stratum code; refer to Indian Time Use Survery for more details.
2. The first 11 columns identify the surveyed household, the next 5 columns inform the survey metadata, the next 18 columns detail informant's response, and the last column assigns a weight to this household.

---

## Individual Data

File: individual.csv
Tag: Demographic particulars of all the household members.
Columns:
- survey_year: 2024
- fsu_serial_no: first stage unit serial number
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- nss_region: National Service Scheme region code (refer to List of NSS Regions)
- district: district code (refer to List of States and Districts)
- stratum: stratum code (definition data mismatch; refer to Indian Time Use Survery for more details)
- sub_stratum: sub stratum code (definition data mismatch; refer to Indian Time Use Survery for more details)
- sub_round: survey round
    - 1: jan - mar
    - 2: apr - jun
    - 3: jul - sep
    - 4: oct - dec
- fod_sub_region: Field Operational Division of National Sample Survey Office (refer to List of FOD Sub-Regions)
- nsc: number of first stage units surveyed within a stratum x substratum for each state x sector
- household_id: household identity code
- individual_id: individual identity code
- response_code: individual response
    - 1: cooperative
    - 2: non-cooperative
- day_of_week: survey day of the week
    - 1: monday
    - 2: tuesday
    - 3: wednesday
    - 4: thursday
    - 5: friday
    - 6: saturday
    - 7: sunday
- type_of_day: survey day type
    - 1: routine day
    - 2: non-routine day
- relation_to_head: individual's relationship to the head of the house
    - 1: self
    - 2: spouse of head
    - 3: married child
    - 4: spouse of married child
    - 5: unmarried child
    - 6: grandchild -6,
    - 7: father/mother/father-in-law/mother-in-law
    - 8: brother/sister/brother-in-law/sister-in-law/other relatives
    - 9: servants/employees/other non-relatives
- gender: individual's gender
    - 1: male
    - 2: female
    - 3: transgender
- age: individual's age
- marital_status: individual's martial status
    - 1: never married
    - 2: currently married
    - 3: widowed
    - 4: divorced/separated
- education_level: individual's education level
    - 1: not literate
    - 2: literate: below primary
    - 3: primary
    - 4: upper primary/middle
    - 5: secondary
    - 6: higher secondary
    - 7: diploma /certificate course (up to secondary)
    - 8: diploma/certificate course (higher secondary)
    - 10: diploma/certificate course(graduation & above)
    - 11: graduate
    - 12: post graduate and above
- employment_status: individual's employment status
    - 11: working as own account worker in household enterprise
    - 12: working as employer in household enterprise
    - 21: working as helper in household enterprise (unpaid family worker)
    - 31: working as regular salaried/wage employee
    - 41: working as casual wage labour in public works
    - 51: working as casual wage labour in other types of work
    - 81: did not work but was seeking and/or available for work
    - 91: attending educational institution
    - 92: attending domestic duties only
    - 93: attending domestic duties and is also engaged in unpaid household enterprise for household use
    - 94: rentiers, pensioners, remittance recipients, etc.
    - 95: not able to work due to disability
    - 97: others (including begging, prostitution, etc.)
- industry: 2-digit code (excluding 98) as per National Industrial Classification (NIC) 2008 (refer to List of National Industrial Classifications)
- weight: survey weight assigned to the individual

#### Note
1. All missing data is represented by 99999.
2. Definition data mismatch for stratum and sub stratum code; refer to Indian Time Use Survery for more details.
3. The first 12 columns identify the surveyed individual, the next 4 columns inform the survey metadata, the next 6
columns detail individual's response, and the last column assigns a weight to this individual.

---

## Time-Use Data

File: timeuse.csv
Tag: Particulars of activities for each household member of age 6 years and above from 4:00 AM on the day before the date of interview to 4:00 AM on the day of the interview.
Columns:
- survey_year: 2024
- fsu_serial_no: first stage unit serial number
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- nss_region: National Service Scheme region code (refer to List of NSS Regions)
- district: district code (refer to List of States and Districts)
- stratum: stratum code (definition data mismatch; refer to Indian Time Use Survery for more details)
- sub_stratum: sub stratum code (definition data mismatch; refer to Indian Time Use Survery for more details)
- sub_round: survey round
    - 1: jan - mar
    - 2: apr - jun
    - 3: jul - sep
    - 4: oct - dec
- fod_sub_region: Field Operational Division of National Sample Survey Office (refer to List of FOD Sub-Regions)
- nsc: number of first stage units surveyed within a stratum x substratum for each state x sector
- household_id: household identity code
- individual_id: individual identity code
- activity_code: activity code as per International Classification of Activities for Time Use Statistics 2016 (refer to Appendix C of the ITUS 2024 report)
- time_from: activity start time
- time_to: activity end time
- location: location where the activity was performed
    - 1: within premises of the dwelling unit of the selected household
    - 2: outside premises of the dwelling unit of the selected household in fixed location
    - 3: outside premises of the dwelling unit of the selected household in non-fixed location
- labour_type: type of labour
    - unpaid work
        - 1: self development/self care/self maintenance, etc.
        - 2: care for children, sick, elderly, differently-abled persons in own households
        - 3: production of other services (except care activities as covered in code 02) for own consumption
        - 4: production of goods for own consumption
        - 5: voluntary work for production of goods in households
        - 6: voluntary work for production of services in households
        - 7: voluntary work for production of goods in market/non-market units
        - 8: voluntary work for production of services in market/non-market units
        - 9: unpaid trainee work for production of goods
        - 10: unpaid trainee work for production of services
        - 11: other unpaid work for production of goods
        - 12: other unpaid work for production of services
    - paid work
        - 13: self-employment for production of goods
        - 14: self-employment for production of services
        - 15: regular wage/salary for production of goods
        - 16: regular wage/salary for production of services
        - 17: casual labour for production of goods
        - 18: casual labour for  production of services
- enterprise_type: type of enterprise
    - 1: proprietary
    - 2: partnership
    - 3: government/local body
    - 4: autonomous Bodies
    - 5: public/private limited company
    - 6: cooperative  societies
    - 7: trust/other non-profit institutions
    - 8: employer’s households (i.e., private households employing maid servant, watchman, cook,etc.)
    - 9: others
- multiple: whether multiple activities were performed in the same time slot
    - 1: yes
    - 2: no
- simultaneous: if multiple activities were performed, whether the activities were performed simultaneously
    - 1: yes
    - 2: no
- major: whether the activity is a major activity
    - 1: major
    - 2: minor
- weight: survey weight assigned to the individual

#### Note
1. All missing data is represented by 99999.
2. Definition data mismatch for stratum and sub stratum code; refer to Indian Time Use Survery for more details.
3. The first 12 columns identify the surveyed individual, the next 9 columns detail individual's time use, and the last column assigns a weight to this individual.