# EncoderTest
Very simple TimedRobot to test sensors on.

This was generated through the `WPILib: Create a new project` command in VSCode. All the smarts are in `Robot.java`.

Points of interest:

* `vendordeps/Phoenix.json` brings in the third party dependencies for the SRX which are in the `com.ctre.phoenix.motorcontrol.can.WPI_TalonSRX` package.
* The robot just passes the position of the two joysticks straight to the differentialdrive.
* Use the [`WPI_TalonSRX`](https://www.ctr-electronics.com/downloads/api/java/html/classcom_1_1ctre_1_1phoenix_1_1motorcontrol_1_1can_1_1_w_p_i___talon_s_r_x.html) class to control a Talon. It implements `SpeedController` so can be used in a drive, and also inherits from [`TalonSRX`](https://www.ctr-electronics.com/downloads/api/java/html/classcom_1_1ctre_1_1phoenix_1_1motorcontrol_1_1can_1_1_talon_s_r_x.html) so you get access to `getSensorCollection`
