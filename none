import requests

def fetch_data(phone_number):
    url = f"https://api.call.teamxdraco.my.id/all-in-one.php?phone={phone_number}"
    response = requests.get(url)
    if response.status_code == 200:
        return response.json()
    else:
        return None

def main():
    phone_number = input("Enter Bangladeshi phone number (without country code and 0): ")
    data = fetch_data(phone_number)
    if data:
        print(data)
    else:
        print("Failed to fetch data.")

if __name__ == "__main__":
    main()
