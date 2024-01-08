import time
from selenium import webdriver
from selenium.webdriver.common.keys import Keys

class EHealth:
    def __init__(self, url):
        self.url = url
        self.driver = webdriver.Firefox()

    def visit_ehealth_site(self):
        self.driver.get(self.url)

    def create_patient_account(self, username, password):
        time.sleep(1)
        username_input = self.driver.find_element_by_name("username")
        username_input.send_keys(username)

        password_input = self.driver.find_element_by_name("password")
        password_input.send_keys(password)

        signup_button = self.driver.find_element_by_id("signup-button")
        signup_button.click()

    def view_medical_record(self):
        view_record_button = self.driver.find_element_by_id("view-record-button")
        view_record_button.click()

    def consult_with_doctor(self):
        consult_button = self.driver.find_element_by_id("consult-button")
        consult_button.click()

if __name__ == "__main__":
    ehealth = EHealth("http://ehealth.com")
    ehealth.visit_ehealth_site()
    ehealth.create_patient_account("johndoe", "password123")
    ehealth.view_medical_record()
    ehealth.consult_with_doctor()
