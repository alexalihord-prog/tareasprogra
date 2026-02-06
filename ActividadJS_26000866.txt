let dia = parseInt(prompt("Ingresa tu dia de nacimiento:"));
let mes = parseInt(prompt("Ingresa tu mes de nacimiento:"));

function obtenerSigno(d, m) 
{
if ((m == 3 && d >= 21) || (m == 4 && d <= 19)) return "Aries";
if ((m == 4 && d >= 20) || (m == 5 && d <= 20)) return "Tauro";
if ((m == 5 && d >= 21) || (m == 6 && d <= 20)) return "Geminis";
if ((m == 6 && d >= 21) || (m == 7 && d <= 22)) return "Cancer";
if ((m == 7 && d >= 23) || (m == 8 && d <= 22)) return "Leo";
if ((m == 8 && d >= 23) || (m == 9 && d <= 22)) return "Virgo";
if ((m == 9 && d >= 23) || (m == 10 && d <= 22)) return "Libra";
if ((m == 10 && d >= 23) || (m == 11 && d <= 21)) return "Escorpio";
if ((m == 11 && d >= 22) || (m == 12 && d <= 21)) return "Sagitario";
if ((m == 12 && d >= 22) || (m == 1 && d <= 19)) return "Capricornio";
if ((m == 1 && d >= 20) || (m == 2 && d <= 18)) return "Acuario";
if ((m == 2 && d >= 19) || (m == 3 && d <= 20)) return "Piscis";
return "Fecha no válida";
}

if (!isNaN(dia) && !isNaN(mes)) 
{
let resultado = obtenerSigno(dia, mes);
alert("Tu signo zodiacal es el siguiente: " + resultado);
} 
else 
{
alert("Fecha no válida");
}