class Calculadora
   attr_accessor :valor1, :valor2
   
   def initialize()
  @valor1 = 0
	@valor2 = 0
   end
   
   def somar
	return @valor1 + @valor2
   end
   
   def dividir
	return @valor1 / @valor2
   end

   def subtrair
	return @valor1 - @valor2
   end

   def multiplicar
	return @valor1 * @valor2
   end
end

	calculadora = Calculadora.new()

	puts "\n\n Diga qual operação simples de matemática você quer fazer ... "
	resp = gets.chop.downcase
	sleep 1

if resp == "soma"

	puts "\n\n Diga qual soma você quer fazer ! "
	sleep 1

	puts "\n Digite o primeiro valor:\n "
	calculadora.valor1 = gets.chop.to_f
	sleep 0.5
	
	puts "\n Digite o segundo valor:\n "
	calculadora.valor2 = gets.chop.to_f
	sleep 0.9

	puts "\n A soma de "
	print calculadora.valor1
	print " + "
	print calculadora.valor2
	print " é igual a: \n "
	sleep 1

	puts calculadora.somar
	sleep 3

elsif resp == "subtração"

	puts "\n\n Qual valor você quer subtrair ? "
	puts "\n Primeiro valor: "
	calculadora.valor1 = gets.chop.to_f
	sleep 0.5
	
	puts "\n Digite o segundo valor: "
	calculadora.valor2 = gets.chop.to_f
	sleep 0.9

	puts "\n A subtração de "
	print calculadora.valor1
	print " - "
	print calculadora.valor2
	print " é igual a:\n "
	sleep 1
	
	puts calculadora.subtrair
	sleep 2

elsif resp == "multiplicação"

	puts "\n\n Quais valores você quer multiplicar ? "
	sleep 0.5
	
	puts "\n Primeiro valor: "
	calculadora.valor1 = gets.chop.to_f
	sleep 0.5
	
	puts "\n Digite o segundo valor: "
	calculadora.valor2 = gets.chop.to_f
	sleep 0.9
	
	puts "\n A multiplicação de "
	print calculadora.valor1
	print " * "
	print calculadora.valor2
	print " é igual a:\n "

	puts calculadora.multiplicar
	sleep 2

elsif resp == "divisão"

	puts "\n\n Qual divisão você quer fazer ? "
	sleep 0.5
	
	puts "\n Digite o primeiro valor: "
	calculadora.valor1 = gets.chop.to_f
	sleep 0.5
	
	puts "\n Digite o segundo valor: "
	calculadora.valor2 = gets.chop.to_f
	sleep 0.9

	puts "\n A divisão de "
	print calculadora.valor1
	print " / "
	print calculadora.valor2
	print " é igual a:\n "
	sleep 1

	puts calculadora.dividir
	sleep 2

else
	puts " Desculpe, operação não disponível, utilize apenas operações simples de cálculo !!! "
end
	sleep 2