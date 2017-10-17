mport scaleapi

client = scaleapi.ScaleClient('SCALE_API_KEY')

client.create_comparison_task(
    callback_url='http://www.example.com/callback',
    instruction='Do the objects in these images have the same pattern?',
    attachment_type='image',
    attachments=[
        'http://i.ebayimg.com/00/$T2eC16dHJGwFFZKjy5ZjBRfNyMC4Ig~~_32.JPG',
        'http://images.wisegeek.com/checkered-tablecloth.jpg'
    ],
    choices=['yes', 'no']
) 
