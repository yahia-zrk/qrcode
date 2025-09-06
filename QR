import qrcode 

def generate_qr_code(text, file_name):
    try:
        qr=qrcode.QRCode(
             version=2,
            error_correction=qrcode.constants.ERROR_CORRECT_L ,
             box_size=10,
             border=3,
        )
        qr.add_data(text)
        qr.make(fit=True)
        img =qr.make_image(fill_color ="#000000")
        img.save(file_name)
        print(f" QR code successfully saved as {file_name}")
    except Exception as e:
        print(f" Error generating QR code: {e}")    
   
   
text = input ("insert your file's link ")

file_name="qr_code.png"
generate_qr_code(text, file_name)
