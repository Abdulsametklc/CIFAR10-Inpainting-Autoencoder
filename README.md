#CIFAR10-Inpainting-Autoencoder

#ENGLISH
This project presents an image inpainting approach for the CIFAR-10 dataset using a custom-built Autoencoder model with a ResNet18-based encoder. Input images are randomly masked by zeroing out ~50% of the pixels, simulating partially missing visual information.

The encoder leverages deep convolutional layers inspired by ResNet18 to learn rich semantic representations, while the decoder reconstructs the original image using a series of transpose convolutions. The model is trained using Mean Squared Error (MSE) loss and optimized with Adam. Visual results demonstrate the model's ability to recover the masked areas convincingly.

📌 Key modules:

Data loading & preprocessing with torchvision.datasets.CIFAR10

Random masking of images using numpy-based strategies

ResNet-inspired encoder, decoder with transposed convolutions

Loss tracking and output visualization

Designed to run efficiently in Google Colab

This project can serve as a foundational experiment in semantic image reconstruction, denoising, and encoder-decoder training with PyTorch.

#TÜRKÇE
Bu proje, CIFAR-10 veri seti üzerinde ResNet18 tabanlı özel bir Autoencoder mimarisi ile görüntü tamamlama (inpainting) işlemi gerçekleştirmektedir. Girdi görüntülerin yaklaşık %50’si rastgele sıfırlanarak maskelenir ve modelin bu eksik bölgeleri yeniden üretmesi beklenir.

Encoder kısmı, ResNet18’den alınan derin konvolüsyonel katmanlar ile semantik özellikleri öğrenir. Decoder kısmı ise bu kodlanmış bilgiyi transpoz konvolüsyonlar ile tekrar orijinal görüntü boyutuna geri döndürür. Model MSELoss ile eğitilir ve Adam optimizasyon algoritması kullanılır. Eğitim sonunda elde edilen görseller, modelin maskelenmiş alanları başarıyla tahmin edebildiğini gösterir.

📌 Öne çıkan bileşenler:

CIFAR-10 veri yükleme ve ön işleme (torchvision.datasets)

NumPy ile maskeleme algoritması

ResNet tabanlı encoder ve transpoz konvolüsyonlu decoder

Eğitim döngüsü ve görsel çıktı üretimi

Google Colab uyumlu çalışma ortamı

Bu çalışma, görsel veri onarımı, gürültü azaltma ve encoder-decoder eğitim mimarileri üzerine temel bir örnek niteliğindedir.
