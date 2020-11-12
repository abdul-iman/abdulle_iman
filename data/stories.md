## greet + show + phones 
* greet
  - utter_how_can_I_help
* buy_phone_laptop{"category":"phone"}
  - product_search_form
  - form{"name":"product_search_form"}
  - form{"name":null}
* goodbye
  - utter_goodbye

## greet + phone_slots_2

* greet
    - utter_how_can_I_help
* buy_phone_laptop{"category":"phone"}
    - slot{"category":"phone"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* goodbye
    - product_search_form
    - slot{"ram":null}
* give_information
    - product_search_form
    - slot{"ram":null}
* give_information
    - product_search_form
    - slot{"ram":8}
* give_information
    - product_search_form
    - slot{"battery":6000}
* give_information
    - product_search_form
    - slot{"camera":50}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":500}
* goodbye
    - utter_goodbye
* out_of_scope
  - action_my_fallback


## New Story2 + phone_slots

* greet
    - utter_how_can_I_help
    - slot{"category":"phone"}
* buy_phone_laptop{"category":"phone"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* give_information
    - product_search_form
    - slot{"ram":10}
* give_information
    - product_search_form
* give_information
    - product_search_form
    - slot{"camera":34}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":3400}
* goodbye
    - utter_goodbye


## greet + fallback + search 

* greet
    - utter_how_can_I_help
* goodbye
    - action_my_fallback
    - slot{"category":"laptop"}
* buy_phone_laptop{"category":"laptop"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* give_information
    - product_search_form
    - slot{"ram":6}
* give_information
    - product_search_form
    - slot{"battery_backup":"12 hours"}
* give_information
    - product_search_form
    - slot{"storage_capacity":"512 GB"}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":505}
* out_of_scope
    - action_my_fallback
    - slot{"category":"laptop"}
* latest_news_phones_laptops{"category":"laptop"}
    - action_show_latest_news
* goodbye
    - utter_goodbye

## greet + slots_laptops

* greet
    - utter_how_can_I_help
    - slot{"category":"laptop"}
* buy_phone_laptop{"category":"laptop"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* give_information
    - product_search_form
    - slot{"ram":8}
* give_information
    - product_search_form
    - slot{"battery_backup":"8 hours"}
* give_information
    - product_search_form
    - slot{"storage_capacity":"256 GB"}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":1800}



## New Story + laptop_slots
* greet
    - utter_how_can_I_help
    - slot{"category":"laptop"}
* buy_phone_laptop{"category":"laptop"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* give_information
    - product_search_form
    - slot{"ram":16}
* give_information
    - product_search_form
    - slot{"battery_backup":13}
* give_information
    - product_search_form
    - slot{"storage_capacity":512}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":1200}

## New Story3+ phone look up

    - slot{"category":"phone"}
* buy_phone_laptop{"category":"phone"}
    - product_search_form
    - form{"name":"product_search_form"}
    - slot{"requested_slot":"ram"}
* give_information
    - product_search_form
    - slot{"ram":12}
* give_information
    - product_search_form
    - slot{"battery":3500}
* give_information
    - product_search_form
    - slot{"camera":30}
* give_information
    - product_search_form
    - form{"name":null}
    - slot{"budget":2000}

## greet + latest + news
* greet
  - utter_how_can_I_help
* latest_news_phones_laptops{"category":"phone"}
  - action_show_latest_news
* goodbye
  - utter_goodbye

## out_of_scope_intent
* out_of_scope
  - action_my_fallback

## out_of_scope_intent
* out_of_scope
  - action_my_fallback