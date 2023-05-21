# Task 3: Password Policy

- Install the "libpam-pwquality" package if not already installed.
- Configure the system to require passwords with at least 10 characters, including at least 
one uppercase letter, one lowercase letter, and one digit.

<img width="608" alt="3 - Task3_page-0001" src="https://github.com/naveenedoth/MindEmpowered-Linux/assets/94816256/6c467348-9007-400b-8b5d-41812732c0ac">

<img width="600" alt="3 - Task3_page-0002" src="https://github.com/naveenedoth/MindEmpowered-Linux/assets/94816256/2a7df864-9ce5-456e-b1a5-7258bb9e1c6c">

<b>We write ``password   requisite   pam_pwquality.so retry=3 minlen=10 ucredit=-1 lcredit=-1 dcredit=-1`` inside <i>/etc/pam.d/common-password</i> file after the `nano` comand.</b><br /><br />


 - Configure the system to remember the last 5 passwords and prevent users from reusing 
them.

<b>We write ``password   required   pam_unix.so obscure sha512 remember=5`` inside <i>/etc/pam.d/common-password</i> file after the `nano` comand.</b>
<br /><br />

- Take a screenshot of the "pam-config --get-parameters" command output and submit it.

<img width="416" alt="3 - Task3_page-0003" src="https://github.com/naveenedoth/MindEmpowered-Linux/assets/94816256/9164b369-953b-43df-8a0b-d2ffdcdfd770">
