# sensor_package/sensor_simulator.py
"""
Modul untuk simulasi sensor suhu dan kelembapan.
"""

import random

def generate_temperature():
    """
    Menghasilkan suhu acak dalam rentang 18 - 35 derajat Celsius.
    """
    return round(random.uniform(18.0, 35.0), 2)

def generate_humidity():
    """
    Menghasilkan kelembapan acak dalam rentang 30 - 70 persen.
    """
    return round(random.uniform(30.0, 70.0), 2)

def get_sensor_data():
    """
    Mengembalikan data sensor suhu dan kelembapan sebagai tuple.
    """
    suhu = generate_temperature()
    kelembapan = generate_humidity()
    return suhu, kelembapan
