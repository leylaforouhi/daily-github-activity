import datetime
import random

def generate_daily_report():
    today = datetime.date.today()
    numbers = [random.randint(1, 100) for _ in range(5)]
    total = sum(numbers)

    report = (
        f"Daily Report - {today}\n"
        f"Generated Numbers: {numbers}\n"
        f"Total: {total}\n"
    )

    return report

if __name__ == "__main__":
    print(generate_daily_report())
