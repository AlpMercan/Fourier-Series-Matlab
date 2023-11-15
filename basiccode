clc
clear

t = linspace(0, 1, 1000);  
k_values = -2:2;          
x = zeros(size(t));
for k = k_values
    if k == 0
        an = 1;  
    else
        an = (2*exp(-1i*pi*k) - exp(-2*1i*pi*k) - 1) / (2*1i*pi*k);
    end
    
    multiplier = exp(1i*k*t*pi);

    x = x + an * multiplier;
end

figure;
plot(t, real(x));  
title('Fourier Series Approximation');
xlabel('Time');
ylabel('Function Value');
