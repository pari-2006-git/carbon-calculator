<?php
$conn = new mysqli("localhost", "root", "", "carbon_db");

if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}

$name = $_POST['name'];
$electricity = $_POST['electricity'];
$travel = $_POST['travel'];

$carbon = ($electricity * 0.5) + ($travel * 0.2);

$sql = "INSERT INTO users (name, electricity, travel, carbon)
        VALUES ('$name', '$electricity', '$travel', '$carbon')";

if ($conn->query($sql)) {
    echo "<h2>Your Carbon Footprint: $carbon</h2>";
} else {
    echo "Error: " . $conn->error;
}
?>