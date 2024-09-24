# class24-09-2024
% Definir los rangos de x1 y x2
x1 = linspace(0, 3, 100); % Rango para x1
% Ecuaciones
x2_1 = (2 - 1.0001 * x1) / 1.0000; % Para la primera ecuación
x2_2 = (2 - 1.0000 * x1) / 1.0000; % Para la segunda ecuación
% Graficar las ecuaciones
figure;
hold on; % Mantener la gráfica actual
plot(x1, x2_1, 'r', 'LineWidth', 2); % Primera ecuación en rojo
plot(x1, x2_2, 'b', 'LineWidth', 2); % Segunda ecuación en azul
% Añadir detalles a la gráfica
xlabel('x1');
ylabel('x2');
title('Gráfica de las ecuaciones');
legend('1.0001x1 + 1.0000x2 = 2', '1.0000x1 + 1.0000x2 = 2');
grid on; % Activar la cuadrícula
axis equal; % Igualar los ejes
hold off; % Liberar la gráfica actual
