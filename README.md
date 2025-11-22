# chirp_august_ble_connection
Pulls the necessary information from the Chirp Access GraphQL API to then do offline authentication to an august smart lock. Used for custom home automation.

# How to Use

1. Create a config.json file with the following items:

```
{
    "username": "YOUR CHIRP EMAIL HERE",
    "password": "YOUR CHIRP PASSWORD HERE"
}

```

2. Run extract_lock_info.ipynb
  - You will receive an email with your verification code needed to move forward. Go to your email and place it in the input that pops up.

3. You will now have a file called door_lock.json. This contains all the information needed to directly auth to the lock using ble and the phenomenal yalexs-ble and bleak modules.

4. Run the jupyter notebook lock_unlock_test.ipynb.
  - You control what operation is being done with lock_cmd