# co6<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>My Courier Delivery & My Ride</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <h1>My Courier Delivery & My Ride</h1>
  </header>

  <div class="display-area" id="displayArea">Add display</div>

  <main>
    <section id="courierSection">
      <h2>Courier</h2>
      <button onclick="toggleSection('courierDetails')">Open</button>
      <div id="courierDetails" class="hidden">
        <label>Location: </label>
        <input type="text" id="courierLocation" placeholder="Enter location" />
        <div class="sendReceive">
          <button onclick="courierSendReceive('send')">Send</button>
          <button onclick="courierSendReceive('receive')">Receive</button>
        </div>
        <div id="courierVehicleOptions" class="hidden">
          <h3>Choose Vehicle</h3>
          <button onclick="selectCourierVehicle('Bike')">Bike</button>
          <button onclick="selectCourierVehicle('Auto')">Auto</button>
          <button onclick="selectCourierVehicle('Car')">Car</button>
          <button onclick="selectCourierVehicle('Mini Auto')">Mini Auto</button>
          <button onclick="selectCourierVehicle('Lorry')">Lorry</button>
        </div>
      </div>
    </section>

    <section id="rideBookingSection">
      <h2>Ride Booking</h2>
      <button onclick="toggleSection('rideBookingDetails')">Open</button>
      <div id="rideBookingDetails" class="hidden">
        <label>Pickup Location: </label>
        <input type="text" id="rideLocation" placeholder="Enter location" />
        <h3>Select Ride Type</h3>
        <button onclick="selectRide('Bike')">Bike</button>
        <button onclick="selectRide('Auto')">Auto</button>
        <button onclick="selectRide('Car')">Car</button>
      </div>
    </section>

    <section id="rentalVehicleSection">
      <h2>Rental Vehicle</h2>
      <button onclick="toggleSection('rentalDetails')">Open</button>
      <div id="rentalDetails" class="hidden">
        <div class="rentalType">
          <h3>Self</h3>
          <button onclick="toggleSection('selfVehicles')">Open</button>
          <div id="selfVehicles" class="hidden">
            <button onclick="selectRentalVehicle('Bike')">Bike</button>
            <button onclick="selectRentalVehicle('Car')">Car</button>
          </div>
        </div>
        <div class="rentalType">
          <h3>Driver</h3>
          <button onclick="toggleSection('driverVehicles')">Open</button>
          <div id="driverVehicles" class="hidden">
            <button onclick="selectRentalVehicle('Bike')">Bike</button>
            <button onclick="selectRentalVehicle('Car')">Car</button>
            <button onclick="selectRentalVehicle('Bus')">Bus</button>
            <button onclick="selectRentalVehicle('Van')">Van</button>
            <button onclick="selectRentalVehicle('Jeep')">Jeep</button>
          </div>
        </div>
      </div>
    </section>
  </main>

  <script src="script.js"></script>
</body>
</html>
