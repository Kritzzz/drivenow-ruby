Installation
=
    gem install 'drivenow'

Example
=
	require 'drivenow'

	puts "Available cities: #{Drivenow::Agent.cities.keys.inspect}" 

	# get all available cars
	cars = Drivenow::Agent.new(:city => :muenchen).cars

	car = cars.first
	puts car.json.inspect
	puts car.name
	puts car.city
	puts car.address.inspect
	puts car.automatic?
	puts car.license_plate
	puts car.model
	puts car.position.inspect
	puts car.fuel_state
	puts car.clean
	puts car.latitude
	puts car.longitude
