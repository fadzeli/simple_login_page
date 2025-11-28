<?php
/**
 * Simple ToyyibPay CreateBill example
 * Save this file as index.php and run from browser or CLI
 */

$secretKey = "wuvd5kaj-nc90-1w1j-j303-c2t3dwpm8a94";       // tukar dengan key sebenar
$categoryCode = "t9udgffy"; // tukar dengan category code anda

// Data untuk create bill
$data = [
    'userSecretKey'            => $secretKey,
    'categoryCode'             => $categoryCode,
    'billName'                 => 'Order Testing',
    'billDescription'          => 'Testing API createBill',
    'billPriceSetting'         => 1,      // 1 = editable price or 0 = fixed price
    'billPayorInfo'            => 1,
    'billAmount'               => '100',  // RM1.00 (Toyyibpay guna sen 100 = RM1.00)
    'billReturnUrl'            => 'https://yourdomain.com/return',
    'billCallbackUrl'          => 'https://yourdomain.com/callback',
    'billExternalReferenceNo'  => 'TEST-' . time(),
    'billTo'                   => 'Testing User',
    'billEmail'                => 'customer@gmail.com',
    'billPhone'                => '0123456789'
];

// API URL (Production)
// $url = 'https://toyyibpay.com/index.php/api/createBill';

// Sandbox mode (enable jika guna staging)
$url = 'https://dev.toyyibpay.com/index.php/api/createBill';

// Execute CURL
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_POST, 1);
curl_setopt($ch, CURLOPT_POSTFIELDS, http_build_query($data));
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);

$response = curl_exec($ch);
curl_close($ch);

$result = json_decode($response, true);

// Debug output
echo "<pre>";
print_r($result);
echo "</pre>";

// Jika berjaya, buka URL bil automatik
if (isset($result[0]['BillCode'])) {
    $billCode = $result[0]['BillCode'];
    $paymentUrl = "https://toyyibpay.com/$billCode";
    echo "<a href='$paymentUrl' target='_blank'>Klik untuk buat pembayaran</a>";
} else {
    echo "Create Bill Failed. Check data or keys.";
}
