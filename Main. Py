
# Classroom Electricity Waste Tracker

classroom_list = []
appliance_list = []
reporter_list = []


def add_report():
    print("\n--- Report Electricity Wastage ---")
    classroom = input("Enter classroom number: ")
    appliance = input("Enter appliance (fan/light/other): ")
    reporter = input("Enter your name: ")

    classroom_list.append(classroom)
    appliance_list.append(appliance)
    reporter_list.append(reporter)

    print("Report submitted successfully!")


def view_reports():
    print("\n--- Electricity Wastage Reports ---")

    if len(classroom_list) == 0:
        print("No reports have been submitted.")
    else:
        for i in range(len(classroom_list)):
            print("\nReport Number:", i + 1)
            print("Classroom:", classroom_list[i])
            print("Appliance:", appliance_list[i])
            print("Reported By:", reporter_list[i])


def show_summary():
    fan_count = 0
    light_count = 0
    other_count = 0

    for i in range(len(appliance_list)):
        if appliance_list[i] == "fan":
            fan_count += 1
        elif appliance_list[i] == "light":
            light_count += 1
        else:
            other_count += 1

    print("\n--- Summary ---")
    print("Total Reports:", len(classroom_list))
    print("Fan Reports:", fan_count)
    print("Light Reports:", light_count)
    print("Other Reports:", other_count)


def main():
    while True:
        print("\n--- CLASSROOM ELECTRICITY WASTE TRACKER ---")
        print("1. Submit a report")
        print("2. View reports")
        print("3. View summary")
        print("4. Exit")

        choice = input("Enter your choice: ")

        if choice == "1":
            add_report()
        elif choice == "2":
            view_reports()
        elif choice == "3":
            show_summary()
        elif choice == "4":
            print("Thank you!")
            break
        else:
            print("Invalid choice!")


main()
