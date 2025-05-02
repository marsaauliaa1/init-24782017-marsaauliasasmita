# main_package/main_24782017.py
"""
Modul utama untuk menampilkan data sensor suhu dan kelembapan dari sensor_simulator.
"""

from sensor_package import sensor_simulator

def main():
    print("SMART HOME - Monitor Suhu dan Kelembapan")
    suhu, kelembapan = sensor_simulator.get_sensor_data()
    print(f"Suhu: {suhu}°C")
    print(f"Kelembapan: {kelembapan}%")

if __name__ == "__main__":
    main()
